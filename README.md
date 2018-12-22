# Islandora PID Alias

## Introduction

A first attempt at addressing https://github.com/Islandora-CLAW/CLAW/issues/822. Create a URL alias for a node from its Islandora 7.x path (e.g. `/islandora/PID`), if the PID field is populated in the Drupal 8 node. If the PID field is not present or not populated, it does nothing.

## Requirements

* [Islandora](https://github.com/Islandora-CLAW/islandora) a.k.a. CLAW

## Installation

1. Clone this repo into your Islandora's `drupal/web/modules/contrib` directory.
1. Enable the module either under the "Admin > Extend" menu or by running `drush en -y islandora_pid_alias`.

## Usage

There is no user interface to this module. It simply creates a URL alias from `/islandora/object/PID` to `/node/NID` if the required conditions as describe in the "Introduction" are met.

## Configuration

None.

## Current maintainer

* [Mark Jordan](https://github.com/mjordan)

## License

[GPLv2](http://www.gnu.org/licenses/gpl-2.0.txt)
