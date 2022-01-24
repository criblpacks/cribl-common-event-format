# Cribl Pack for Common Event Format (CEF)
----

The Cribl Pack for Common Event Format reshapes your CEF messages into formats that are easily processed by consuming systems. For example, CEF to JSON. Additionally, the pack can process mapping of the custom string and custom number field values and labels into respective fields.

```
The pack turns this:
cs4=103.6.32.100 cs4Label=clientIPAddress

into this:
clientIPAddress=103.6.32.100
```

## Installation
---
1. Get the bits.
   1. Download the most recent .crbl file from the repo [releases page](https://github.com/criblpacks/cribl-common-event-format/releases).
   2. -or- Install in LogStream via the Github URL for this pack: `https://github.com/criblpacks/cribl-common-event-format.git`
2. Create a Route with with a filter for your CEF events.
3. Select the `Common Event Format (CEF)` pack as the pipeline.
4. Configure the pack `cef_processor` pipeline with the desired output format. K=V, JSON, and CEF-like are pre-configured output options. Enable one of these function groups. **Failure to enable an output configuration will result in functionality similar to the "passthru" pipeline.**


## Release Notes
---
### Version 0.1.0 - 2021-09-17
Initial release


## Contributing to the Pack
---
Discuss this pack on our Community Slack channel [#packs](https://cribl-community.slack.com/archives/C021UP7ETM3).

## Contact
---
The author of this pack is Brendan Dalpe and can be contacted at <bdalpe@cribl.io>.

## License
---
This Pack uses the following license: [`Apache 2.0`](https://github.com/criblio/appscope/blob/master/LICENSE).
