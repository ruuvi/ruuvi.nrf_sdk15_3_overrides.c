# ruuvi.nrf_sdk15_3_overrides.c
Override specific files in nRF5 SDK15.3

# License
MIT, check LICENSE

# Changes
## nrf_bootloader_wdt.c
 - Cap WDT feed timer into 2^20 timer ticks. 
 - Feed WDT after timer has been started.

## nrfx_wdt.c
 - Fix watchdog overflow on multiply by 2^15 / 1000 conversion