# lnav_idcloud
Custom format file for [lnav](https://lnav.org/) to format ForgeRock Identity Cloud logs, currently targeted to formatting the debug logs (source=am-core).

## Prerequisites
* A ForgeRock Identity Cloud tenant with credentials for the Log API.
* Utility for ID Cloud logs [FIDC Debug Tool](vscheuber/fidc-debug-tools)
* [lnav](https://lnav.org/) 

## Installation
`lnav -i forgerock_idcloud_log.json`

## Usage
`./tail.am-core.js. | lnav`
