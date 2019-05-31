# SPPD-Deck-Tracker
South Park Phone Destroyer Deck Tracker

Current Version: v0.90 BETA


Introduction:
============

This is a very basic application meant to run along side South Park Phone Destroyer

At the moment, SECURITY_CODE is a required setting for beta testing, until official release.

Please join the discord: https://discord.gg/m95hg3S

Current supported actions:
  * Tracking Opponent's Deck in real-time, as they play cards
  * Log Match Details
  * Log Locker Rewards
  * Log Pack Rewards
  
Known Issues:
  * Tracking Opponent's Deck does not work on iPhone.


Installation:
==============

For Android:
  * Download and Install Nox
    * Nox: https://www.bignox.com/
  * Run the Deck Tracker
    * Verify your Settings are correct
	* Install the certificate on your local computer
  * Update your Wifi Settings
    * Long-click on Wifi to modify settings
	   * Add a manual proxy using hostname: __my_IP__, port: 8877
  * Navigate and install the certificate at: http://__my_IP__:8877/

For iPhone:
  * Run the Deck Tracker
    * Verify your Settings are correct
	* Install the certificate on your local computer
  * Update your Wifi Settings
	 * Add a manual proxy using hostname: __my_IP__, port: 8877
  * Navigate and install the certificate at: http://__my_IP__:8877/
  * Grant full access to the certificate
	  * Navigate to Settings
		* Search for certificates
		* Find the one you just installed
		* Enable full access


Usage:
================================
  * Complete installion successfully
  * Launch the SPPD Deck Tracker Application
  * Verify the correct network is selected in the SETTINGS tab
  * Click the RUN button (wait ~5 seconds)
  * Play a game, purchase/collect packs and lockers


Files:
============================================
  * CARDS/* - Icons for characters, spells, rewards
  * OUTPUT/* - Log of deck-tracker, matches, packs, lockers


Issues or Feature Requests?
============================================
Open an issue and attach a screenshot of the offending screen.
There's no such thing as a bad feature request.


Roadmap and Milestones:
============================================
	* May 30, 2019 - Initial Commit
	* June 2019 - Card Levels
	* June 2019 - Estimate ELO gained/lost For Win or Loss
	* June 2019 - Deck Building Tab
	* June 2019 - Export Collection
	* July 2019 - Locker Limit Tracking
	* August 2019 - Team Search Tab - A better team search function
		* Search by TVT tier, Average MMR, number of players in a specific range (40-49)
	* August 2019 - Statistics Tab - Win Rate + Epic/Legendary graphs
	* Summer 2018 or Pending Community Approval - Tracking Opponent's Energy
	* TBD - Mouse-over card icon for name
	* TBD - Display HP/ATTACK/OTHER-damage Checkbox