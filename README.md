# AIS.Net Notebooks
A selection of .NET Interactive Notebooks demoing Ais.Net functionality.

## About AIS and AIS.Net 

These demo's use the the Norwegian Coastal Administration's marine Automatic Identification System (AIS) [AIVDM/AIVDO](https://gpsd.gitlab.io/gpsd/AIVDM.html) NMEA message network data (available under [Norwegian license for public data (NLOD)](https://data.norge.no/nlod/en/2.0)) to perform analysis of vessel tracking data, using using [endjin's](https://endjin.com) open source [AIS.Net libraries](https://github.com/ais-dotnet/).


The AIS.NET project contains a series of layers, from a low-level high performance NMEA AIS sentence decoder, to a rich high-level C# 9.0 models of AIS message types, a receiver component that can listen to TCP streams of NMEA sentences and expose them as an `IObservable<string>` of raw sentences or an decoded `IObservable<IAisMessage>`, and finally a Storage Client implementation to persisting the raw NMEA sentence stream to Azure Blob storage for future processing.

![https://github.com/ais-dotnet](https://endjincdn.blob.core.windows.net/assets/ais-dotnet-project-layers.png)

## Licenses

[![GitHub license](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://raw.githubusercontent.com/ais-dotnet/Ais.Net.Receiver/master/LICENSE)

AIS.Net.Receiver is also available under the Apache 2.0 open source license.
 
The Data ingested by the AIS.Net.Receiver is licensed under the [Norwegian license for public data (NLOD)](https://data.norge.no/nlod/en/2.0).

## Project Sponsor

This project is sponsored by [endjin](https://endjin.com), a UK based Microsoft Gold Partner for Cloud Platform, Data Platform, Data Analytics, DevOps, Power BI Partner, and [.NET Foundation Corporate Sponsor](https://dotnetfoundation.org/#corporate-sponsors).

For more information about our products and services, please [contact us](https://endjin.com/contact-us). 

We produce two free weekly newsletters; [Azure Weekly](https://azureweekly.info) for all things about the Microsoft Azure Platform, and [Power BI Weekly](https://powerbiweekly.info).

Keep up with everything that's going on at endjin via our [blog](https://blogs.endjin.com/), follow us on [Twitter](https://twitter.com/endjin), or [LinkedIn](https://www.linkedin.com/company/1671851/).

Our other Open Source projects can be found on [GitHub](https://endjin.com/what-we-do/open-source/).

## Code of conduct

This project has adopted a code of conduct adapted from the [Contributor Covenant](http://contributor-covenant.org/) to clarify expected behavior in our community. This code of conduct has been [adopted by many other projects](http://contributor-covenant.org/adopters/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [&#104;&#101;&#108;&#108;&#111;&#064;&#101;&#110;&#100;&#106;&#105;&#110;&#046;&#099;&#111;&#109;](&#109;&#097;&#105;&#108;&#116;&#111;:&#104;&#101;&#108;&#108;&#111;&#064;&#101;&#110;&#100;&#106;&#105;&#110;&#046;&#099;&#111;&#109;) with any additional questions or comments.