# Venn Diagrams For All

When writing some ABAP code, it typically interacts with other parts of the system via an API.
SAP marks different objects as released, which then is considered "stable".
There are many kinds of objects which can be marked as released, such as, Data Elements, Domains, CDS Views, Object Oriented Interfaces, Object Oriented Classes, and more.

In the beginning(not taking versioning into account), custom(customer) logic written on ABAP Cloud in SAP BTP ABAP Environment can utilize the Released APIs,

![Beginning](./img/beginning.drawio.svg)

Assuming all celestial bodies align, and releases goes into the same releases, then, S/4 HANA Cloud Public Edition, includes the full set of released APIs in ABAP Cloud in SAP BTP ABAP Environment. All objects used in custom developments must be released.

Example: CL_HTTP_DESTINATION_PROVIDER is released in both ABAP Cloud in SAP BTP ABAP Environment and S/4 HANA Cloud Public Edition

Example: CDS View I_BusinessPartner is not part of ABAP Cloud in SAP BTP ABAP Environment, but part of and released in S/4 HANA Cloud Public Edition

All released APIs in S/4 HANA Cloud Public Edition falls into one of these two groups,

![public cloud](./img/cloudcloudpublic.drawio.svg)

In S/4 HANA Cloud Private Edition, there are Released APIs and Classic ABAP, where the developer chooses which kind of development to do.

![public cloud](./img/privateed.drawio.svg)

Then we have,

![public cloud](./img/wehave2.drawio.svg)

<!--
Previously my understanding was,
![public cloud](./img/old.drawio.svg)
-->

But actually its more like

![Foo](./img/foo2.drawio.svg)

Not taking specific releases into account