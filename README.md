# Bosch Rexroth CycloneDX Property Taxonomy, v1.0.0

This is the official Bosch Rexroth property taxonomy for CycloneDX.

For more information about CycloneDX property taxonomies, refer to
their [official documentation](https://github.com/CycloneDX/cyclonedx-property-taxonomy).

<table>
<thead>
    <tr>
        <th>Property</th>
        <th>Description</th>
    </tr>
</thead>
<tbody>
    <tr style="vertical-align: top;">
        <td><b>boschrexroth:additionalCopyrightInformation</b></td>
        <td>The content of additional copyright information (e.g. NOTICE file - Apache License or additional hints in the license text, readme or authors, contributors files).<br><br>Intended for use in <code>components[]/properties</code>.</td>
    </tr>
    <tr style="vertical-align: top;">
        <td><b>boschrexroth:integrationMechanism</b></td>
        <td>Only mandatory if the license is a weak or strong copyleft license (e.g., GPL, LGPL).<br><br>
        Specifies how the component was integrated in the software.<br><br>
		<ul>
		  <li><strong>linkedDynamically</strong> = The component and other components of the software are compiled separately. The generated objects are kept separately (i.e., in separate directories). The component is linked at runtime to form a joint object code. In case of Java, the component is integrated via the import mechanism in Java (i.e. classloader).</li>
		  <li><strong>linkedStatically</strong> = The component and other components of the software are compiled separately, and the generated objects are linked during an offline process to create a single software component to be distributed.</li>
		  <li><strong>snippet</strong> = A part of the source code of the component is added to the source code of the software.</li>
		  <li><strong>callOfLinuxKernelServiceViaSystemCall</strong> = The only connection of an application in the user space to the component is the call of a kernel service via a system call. The software and the component are kept separately (i.e., in separate directories).</li>
		  <li><strong>separateComponent</strong> = There is no connection between the component and the software at all. The component is distributed along with the software. The only connection to the component is the call to an executable. The components communicate via the inter-process communication mechanisms only (e.g., via file, signal, socket, message queue, pipe, named pipe, semaphore, shared memory, memory mapped files). A further investigation would be needed for message passing. The component is kept separately from the software (i.e., in separate directories).</li>
		</ul>
		Intended for use in <code>components[]/properties</code>.</td>
		</td>
    </tr>
    <tr style="vertical-align: top;">
        <td><b>boschrexroth:remarksToLicenseObligations</b></td>
        <td>Important information to fulfill the license obligations for a distribution.<br><br>
		E.g.: <i>All advertising materials mentioning features or use of this software must display the corresponding acknowledgement.</i><br><br>		
		Intended for use in <code>components[]/properties</code>.</td>
    </tr>
</tbody>
</table>


## Contributing

These properties are maintained by Bosch Rexroth. Feel free to raise an issue if you have any questions.


## License

Copyright (c) 2023 Bosch Rexroth AG

Licensed under [Apache License 2.0](./LICENSE).
