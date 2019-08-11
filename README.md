# SPPD-Deck-Tracker
South Park Phone Destroyer Deck Tracker

Current Version: v1.02


Introduction:
============

This is a very basic application meant to run along side South Park Phone Destroyer

Please join the discord: https://discord.gg/m95hg3S

Walkthrough of the installation process with Nox: https://youtu.be/zJnpfzSowlE

Current supported actions:
  * Tracking Opponent's Deck in real-time, as they play cards
  * Log Match Details
  * Log Locker Rewards
  * Log Pack Rewards
  * TVT Bracket Analytics
  * Estimated ELO gained/lost For Win/Loss
  * Locker Limit Tracking (When it resets and how far along you are)
  * Deck Building Tab (Build and store as many decks as you want)
  * Export your entire collection in an easy-to-read format
  * Tracking both player's energy
  
Known Issues:
  * Tracking Opponent's Deck does not work on iPhone.


Installation:
==============

Installation Video [I need to update this with some missing parts]: https://youtu.be/zJnpfzSowlE

Before installation, you need to install WinPcap from https://www.winpcap.org/

After downloading the SPPD Deck Tracker, you may need to Unblock the DLLs in libpcap and libpcap/_platform: https://i.imgur.com/dKJEAfd.png

For Android:

Option 1) Nox Android Emulator (Preferred)
  * Download and Install Nox
    * Nox: https://www.bignox.com/
  * Run the Deck Tracker
    * Verify your Settings are correct
	* Install the certificate on your local computer
  * Update your Wifi Settings on the Android Emulator (Nox)
    * Long-click on Wifi to modify settings
	   * Add a manual proxy using hostname: __my_IP__, port: 8877
  * Navigate and install the certificate at: http://__my_IP__:8877/
     * VPN and Apps, Set Lock Screen

Option 2) BlueStacks Android Emulator
  * If you insist on using Bluestacks, download, install and ROOT Bluestacks
    * Root directions here: https://www.youtube.com/watch?v=hneUrKMMaDc
  * Run the Deck Tracker
    * Verify your Settings are correct
	* Install the certificate on your local computer
  * Click the "Set BlueStacks Proxy" Button in the Settings Tab
    * Download and install Platform Tools: https://developer.android.com/studio/releases/platform-tools
	* Add platform-tools to the PATH in environment variables
    * Now you need to copy your PEM-encoded CA file to the system partition, like:
	  * Open a command prompt and navigate to your deck tracker folder. Locate the file "269953fb.0"
	
      * $ adb root
	  * $ adb shell mount -o remount,rw /system
      * $ adb push 269953fb.0 /etc/security/cacerts/
      * $ adb shell chmod 644 /etc/security/cacerts/269953fb.0
	  * $ adb shell mount -o remount,ro /system
	  
	  OR
	  
	  * adb connect 127.0.0.1:5555
	  * adb -t X push 269953fb.0 /sdcard/
	     * (where X is the transport ID defined in `adb devices -l`)
	  * adb -t X shell
	  * $> su
	  * $> mount -o remount,rw /system
	  * $> mv /sdcard/269953fb.0 /etc/security/cacerts/
	  * $> chmod 644 /etc/security/cacerts/269953fb.0
	  * $> mount -o remount,ro /system
    * If you get an error about "Invalid License", then you have to reinstall SPPD. (something about rooting the device makes it happen)

For iPhone:
  * Run the Deck Tracker
    * Verify your Settings are correct
	* Install the certificate on your local computer
  * Update your Wifi Settings on the iPhone
	 * Add a manual proxy using hostname: __my_IP__, port: 8877
  * Navigate and install the certificate at: http://__my_IP__:8877/
  * Grant full access to the certificate
	  * Navigate to Settings
		* Search for certificates
		* Find the one you just installed
		* Enable full access

Note: I have only verified functionality on:
   * iPhone 5
   * Nox 6.2.8.0 (Android 5)
   * Bluestacks 4 (rooted)
If you have gotten this working on a different device, please let me know.

Usage:
================================
  * Complete installion successfully
  * Launch the SPPD Deck Tracker Application
  * Verify the correct network is selected in the SETTINGS tab
  * Click the RUN button (wait ~5 seconds)
  * Play a game, purchase/collect packs and lockers


Files:
============================================
  * CARDS/* 	- Icons for characters, spells, rewards
  * OUTPUT/* 	- Log of deck-tracker, matches, packs, lockers
  * libpcap/* 	- Library modules for the deck tracker
  * SPPD_Deck_Tracker.exe 	- The primary executable you need to run
  * SETTINGS.txt	- The raw settings file used by the executable


Issues or Feature Requests?
============================================
Open an issue and attach a screenshot of the offending screen.
There's no such thing as a bad feature request.


Roadmap and Milestones:
============================================
	* May 30, 2019 - Initial Commit
	* June 14, 2019 - Estimate ELO gained/lost For Win or Loss
	* June 14, 2019 - Locker Limit Tracking
	* June 21, 2019 - Deck Building Tab
	* June 21, 2019 - Export Collection
	* July 2019 - All Card Levels
	* August 2019 - Team Search Tab - A better team search function
		* Search by TVT tier, Average MMR, number of players in a specific range (40-49)
	* August 2019 - Statistics Tab - Win Rate + Epic/Legendary graphs
	* August 2019 - Tracking Both Player's Energy
	* TBD - Mouse-over card icon for name
	* TBD - Display HP/ATTACK/OTHER-damage Checkbox
