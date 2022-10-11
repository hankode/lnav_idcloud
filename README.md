# lnav_idcloud
Custom format file for [lnav](https://lnav.org/) to format ForgeRock Identity Cloud logs, currently targeted to formatting the debug logs (source=am-core).

## Prerequisites
* A ForgeRock Identity Cloud tenant with credentials for the Log API.
* A utility for tailing ID Cloud logs:
  * [Frodo CLI](https://github.com/rockcarver/frodo-cli)
  * [FIDC Debug Tool](vscheuber/fidc-debug-tools)
* [lnav](https://lnav.org/) 

## Installation
`lnav -i forgerock_idcloud_log.json`

## Usage
  * Using tail_am from FIDC Debug Tool:
  
`./tail_am 2>/dev/null | lnav`

  * Using Frodo:
  
`frodo logs tail <your_host> -l 3 -c am-everything 2>&1 | lnav`
