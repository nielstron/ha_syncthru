[![hacs_badge](https://img.shields.io/badge/HACS-Custom-orange.svg)](https://github.com/custom-components/hacs)

# Syncthru custom component for Home Assistant

A custom component to integrate the Samsung SyncThru printers to Home Assistant.
It automatically determines whether your printer provides a built-in API
and switches to makeshift web scraping in case it can't access any API endpoints.

## Should I install this?

If you tried setting up your Samsung printer via config flow and got an error message
that says that your server does not support the SyncThru API, you may try this package.
It will probably work and display at least some of the available values.

## Why is this not part of HA core? What is the difference?

While the Home Assistant core [already contains a syncthru component](https://home-assistant.io/components/syncthru),
the Home Assistant development guidelines forbid making use of web scraping in any core component.
Hence this is a fork of the core component that enables making use of the web scraping capabilities
of the underlying package [pysyncthru](https://github.com/nielstron/pysyncthru).

## Installation

Add this repository to [hacs](https://hacs.xyz/) or copy the `custom_component/syncthru` file structure into your custom_component directory .

The configuration of this component is exactly the same as for [the core component](https://home-assistant.io/components/syncthru).

## Contributions

Feel free to open Pull Requests here or at
the backend python script [pysyncthru](https://github.com/nielstron/pysyncthru).
