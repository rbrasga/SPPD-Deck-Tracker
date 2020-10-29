# SPPD-Deck-Tracker
South Park Phone Destroyer Deck Tracker

This content is in no way approved, endorsed, sponsored, or connected to South Park Digital Studios, Ubisoft, RedLynx, or associated/affiliated entities, nor are these entities responsible for this content.

Current Version: v2.44

Introduction:
============

This is a very basic application meant to run along side South Park Phone Destroyer.

This 

Please join the discord: https://discord.gg/m95hg3S

**Updated Video Guides** - Thanks to `3LV1N5#0987`
   * iOS Install Guide: https://www.youtube.com/watch?v=ZTl1Go8Fh1Q
   * Android Emulator Install Guide: https://www.youtube.com/watch?v=_ienJRZcSx0
   * Play iOS on PC: https://www.youtube.com/watch?v=elLGcli0Bx8

Current supported actions:
  * Tracking each player's decks
  * Log Match Details
  * Log Locker/Pack Rewards (and filter by value)
  * TVT Bracket Analytics
  * ELO gained/lost For Win/Loss
  * Locker Limit Tracking (When it resets and how far along you are)
  * Deck Building Tab (Build and store as many decks as you want)
    * Supports all themes in a single deck, to more easily communicate multi-theme TVT decks.
  * Export your entire collection in an easy-to-read format
  * Login to iOS account on Android device (see details below)
  * Team Wars History analytics (including export)


Installation:
==============
**Updated Video Guides** - Thanks to `3LV1N5#0987`
   * iOS Install Guide: https://www.youtube.com/watch?v=ZTl1Go8Fh1Q
   * Android Emulator Install Guide: https://www.youtube.com/watch?v=_ienJRZcSx0
   * Play iOS on PC: https://www.youtube.com/watch?v=elLGcli0Bx8

For Android:

Option 1) Nox/MEMU Android Emulator (Preferred)
  * Download and Install (Pick one! Nox or MEMU)
    * Nox: https://www.bignox.com/
	* MEMU: https://www.memuplay.com/
  * Run the Deck Tracker
    * Verify your Settings are correct
	* Install the certificate on your local computer
  * Update your Wifi Settings on the Android Emulator
    * Long-click on Wifi to modify settings
	   * Add a manual proxy using hostname: __my_IP__, port: 8877
	      * __my_IP__ is found in the Deck Tracker SETTINGS Tab.
    * Navigate and install the certificate at: http://__my_IP__:8877/

Option 2) BlueStacks Android Emulator (10 minutes)
  * If you insist on using Bluestacks, download, install and ROOT Bluestacks
    * Root directions here: https://www.youtube.com/watch?v=hneUrKMMaDc
    * Note: If you get an error while launching SPPD about "Invalid License", then you have to reinstall SPPD. (something about rooting the device makes it happen)
  * Download from the app store: "Root Certificate Manager" (phone should be rooted first)
  * Run the Deck Tracker
    * Verify the settings in the (SPPD Deck Tracker) SETTINGS's Tab are correct
	* Install the certificate on your local computer
  * Click the "Set BlueStacks Proxy" Button in the Settings Tab
    * Download the certificate onto bluestacks
	  * Open an internet browser on bluestacks and go to http://__my_IP__:8877/
	  * This is an example link. Your actual IP Address is listed in the deck tracker SETTINGS tab.
	  * Download the certificate, but don't bother trying to install it, because you can't anyways.
	* Now open the app "Root Certificate Manager", and Import the certificate (.cer) file you just downloaded.
	* Now you're ready to use all of the features of the deck tracker.
  * Note: Each time after you set the proxy, you have do a *full restart* of bluestacks
    * Exit Bluestacks by clicking 'Quit' from the bluestacks icon in the system tray (near the clock).
	* Then start it up again - now the proxy is ready to go!

For iOS Devices:
  * Run the Deck Tracker
    * Verify your Settings are correct
	* Install the certificate on your local computer
  * Update your Wifi Settings on the iPhone
	 * Add a manual proxy using hostname: __my_IP__, port: 8877
	    * __my_IP__ is found in the Deck Tracker SETTINGS Tab.
  * Navigate and install the certificate at: http://__my_IP__:8877/
  * Grant full access to the certificate
	  * Navigate to Settings
		* Search for certificates
		* Find the one you just installed
		* Enable full access

Usage:
================================
  * Download all the files by clicking Clone -> Download as Zip, then extract all the files.
  * Launch the SPPD Deck Tracker Application
  * Click the RUN button
  * Start the app SPPD (Do not connect to the deck-tracker after already starting SPPD)
  * Play a game, purchase/collect packs and lockers
  
Alternate Login:
================================


**Updated Video Guides**
   * Play iOS on PC: https://www.youtube.com/watch?v=elLGcli0Bx8

Both iOS and Android accounts to iOS and Android devices are supported. See details below.
  * IOS account to Android Device
    * No username/password needed, but an iOS device IS needed.
    * Connect both (ios device and android device) to the deck tracker.
    * Enable Alternate Login + iOS in the deck tracker SETTINGS tab
    * Then launch SPPD on your iOS device
    * You can now close SPPD on your iOS device
    * Launch the game on your android device - you will automatically log in to your iOS account.
  * Android account to iOS Device
    * Android username/password needed, no Android device is needed.
    * Connect IOS device to the deck tracker.
    * Enable Alternate Login + Android in the deck tracker SETTINGS tab
    * Input your Android Username/Password (password is only required the first time)
    * Then launch SPPD on your iOS device - you will automatically log in to your Android account.

Files:
============================================
  * OUTPUT/* 	- Log of matches, packs, lockers
  * SPPD_Deck_Tracker.exe 	- The primary executable you need to run
  * SETTINGS.txt	- The raw settings file used by the executable


Issues or Feature Requests?
============================================
Open an issue and attach a screenshot of the offending screen.
There's no such thing as a bad feature request.


Roadmap and Milestones:
============================================
	* May 2019 - Initial Commit
	* June 2019 - Estimate ELO gained/lost For Win or Loss
	* June 2019 - Locker Limit Tracking
	* June 2019 - Deck Building Tab
	* June 2019 - Export Collection
	* July 2019 - All Card Levels
	* August 2019 - Tracking Both Player's Energy
	* October 2019 - Automatic Team Bottle Cap Upgrade Tracking
	* TBD - Team Search Tab - A better team search function
		* Search by TVT tier, Average MMR, number of players in a specific range (40-49)
	* TBD - Statistics Tab - Win Rate + Epic/Legendary graphs
	* TBD - Mouse-over card icon for name
	* TBD - Display HP/ATTACK/OTHER-damage Checkbox
