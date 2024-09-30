# SIEM Lab (Azure Sentinel Project)

## Objective

The SIEM Lab project focused on creating a secure environment for simulating and analyzing cyber attacks using Azure Sentinel as a SIEM solution. The primary goal was to ingest and process logs, extract metadata, and generate insights to detect attack patterns. Through this hands-on experience, the project helped build a deeper understanding of network security, attack telemetry, and geolocation-based threat analysis.

### Skills Learned

- Advanced understanding of Azure Sentinel and SIEM implementation.
- Proficiency in PowerShell scripting for log extraction and manipulation.
- Expertise in configuring and analyzing network logs for geolocation data.
- Ability to map and visualize attack patterns based on geographic information.
- Enhanced critical thinking for real-world cyber threat detection and mitigation.

### Tools Used

- **Azure Sentinel**: Configured for log ingestion and visualization of attack data.
- **PowerShell**: Used to develop scripts for extracting and manipulating metadata.
- **Log Analytics Workspace**: Configured for custom log ingestion and field mapping.
- **Telemetry Generation**: Created realistic attack data for analysis and testing.
- **Network Analysis Tools** (e.g., Wireshark): Used to capture and analyze network traffic related to attacks.

## Steps

1. **Developed custom PowerShell scripts**  
   Created scripts to extract metadata from the Windows Event Viewer logs. This metadata included crucial details such as event types, timestamps, and user activities, which were essential for understanding the system's state.

   *Ref 1: PowerShell Script for Log Extraction*  
   ![PowerShell Script Example](imgur_link1)

2. **Forwarded extracted metadata to third-party API**  
   The metadata extracted from Event Viewer logs was sent to an external API for geolocation data enrichment. The API derived information such as latitude, longitude, state/province, and country based on the IP addresses found in the logs.

   *Ref 2: API Response with Geolocation Data*  
   ![API Response Screenshot](imgur_link2)

3. **Configured Log Analytics Workspace**  
   Log Analytics Workspace was set up to ingest and process the custom logs containing geographic information. This involved configuring data inputs, creating custom fields, and mapping the enriched geolocation data.

   *Ref 3: Log Analytics Configuration*  
   ![Log Analytics Workspace Configuration](imgur_link3)

4. **Created custom fields in Log Analytics Workspace**  
   Developed custom fields within Log Analytics to map and display the geolocation data. These fields were used to visualize the geographic distribution of incoming data, allowing better analysis of attack origins.

   *Ref 4: Custom Fields for Geolocation Mapping*  
   ![Custom Fields Example](imgur_link4)

5. **Configured an Azure Sentinel workbook**  
   A custom workbook was created in Azure Sentinel to display brute force RDP attacks on a world map. This visualization provided a global view of attack sources and magnitudes, helping to identify regions with higher attack frequencies.

   *Ref 5: Azure Sentinel Workbook*  
   ![Sentinel Workbook for Global Attack Mapping](imgur_link5)
