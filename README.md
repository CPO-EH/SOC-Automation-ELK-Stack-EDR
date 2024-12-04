# SOC-Automation-ELK-Stack-EDR

## Objective

The SOC Automation & ELK Stack EDR project was designed to simulate a real-world cybersecurity environment where both offensive and defensive measures were implemented. The primary goal was to build a lab for detecting and responding to simulated cyberattacks using the ELK Stack and automated workflows.

### Skills Learned

- Network Threat Detection: Configured ELK Stack for log ingestion, analysis, and alert generation.
- Incident Response: Designed workflows for active response to cyber incidents.
- Automation: Automated alerting and incident ticket creation using integrated tools like osTicket.
- Offensive Security: Simulated cyberattacks using Kali Linux and Mythic C2 to identify weaknesses and 
  validate defense strategies.
- Network Architecture Design: Built a cloud-based infrastructure in Vultr to simulate real-world SOC 
  operations.

### Tools Used

- Elastic Stack (ELK): Elasticsearch, Logstash, and Kibana for log management and analysis.
- Mythic C2: Command-and-control framework for attack simulation and payload delivery.
- osTicket: Ticketing system for incident management and response.
- Fleet Server: Managed endpoint agents for data collection and telemetry.
- Kali Linux: Offensive security platform for attack emulation.
- Vultr: Cloud hosting platform for network architecture deployment.
- Elastic Defend: Endpoint protection solution for detecting and responding to threats in real time.

## Project Walkthrough

- Network Diagram & Attack Lifecycle (Mitre Att&ck Framework)
<div align="center">
  <table>
    <!-- Row 1 -->
    <tr>
      <td align="center">
        <strong>Network Diagram</strong><br>
        <img width="300" alt="Screenshot 1: Network Diagram" src="https://github.com/user-attachments/assets/07b7e03b-e87d-4b66-97e7-83e7339b71f6">
      </td>
      <td align="center">
        <strong>Attack Lifecycle</strong><br>
        <img width="300" alt="Screenshot 2: Attack Lifecycle" src="https://github.com/user-attachments/assets/684acdaf-a0bc-4446-a734-319d331de529">
      </td>
    </tr>
  </table>
</div>


- [ELK Stack server install on UbuntuOS (Vultr Cloud)](https://github.com/techgneek/SOC-Automation-ELK-Stack-EDR/blob/main/ELK%20Stack%20Server%20Install)

<div align="center">
  <table>
    <!-- Row 1 -->
    <tr>
      <td align="center">
        <strong>Download ElasticSearch/Kibana </strong><br>
        <img width="300" alt="Screenshot 1: Starting ElasticSearch Installation" src="https://github.com/user-attachments/assets/56f9ae9f-63f2-4ce2-9d21-46c5dd490c8a">
      </td>
      <td align="center">
        <strong>Installing ElasticSearch </strong><br>
        <img width="300" alt="Screenshot 2: Verifying ElasticSearch Configuration" src="https://github.com/user-attachments/assets/d140e795-f108-4df1-894d-60080dc00899">
      </td>
      <td align="center">
        <strong>Configuring Kibana Settings</strong><br>
        <img width="300" alt="Screenshot 3: Configuring Kibana Settings" src="https://github.com/user-attachments/assets/a4872a0e-7d11-432d-986f-da2524c55793">
      </td>
      <td align="center">
        <strong>Generating Encryption Keys</strong><br>
        <img width="300" alt="Screenshot 4: Firewall Rule Configuration" src="https://github.com/user-attachments/assets/4a4b6b61-acf3-492f-9521-afac95eb150a">
      </td>
    </tr>
    <!-- Row 2 -->
    <tr>
      <td align="center">
        <strong>Configuring Firewalls For ELK Stack Server</strong><br>
        <img width="300" alt="Screenshot 5: Generating Encryption Keys" src="https://github.com/user-attachments/assets/6b562fad-5df6-4247-be1d-fc61bd1a7c69">
      </td>
      <td align="center">
        <strong>Testing Open Ports On Server</strong><br>
        <img width="300" alt="Screenshot 6: ElasticSearch Service Status" src="https://github.com/user-attachments/assets/6f47e70f-660c-47dc-8752-5d1b2f25e279">
      </td>
      <td align="center">
        <strong>Configuring Encryption Keys</strong><br>
        <img width="300" alt="Screenshot 7: Testing Open Ports" src="https://github.com/user-attachments/assets/48926403-441a-4fc0-aae7-b80ab0c703cb">
      </td>
      <td align="center">
        <strong>Completed Kibana Setup</strong><br>
        <img width="300" alt="Screenshot 8: Completed Kibana Setup" src="https://github.com/user-attachments/assets/fe31b04b-12b6-43de-9eff-d83bc673a9b1">
      </td>
    </tr>
  </table>
</div>

- [Windows 2022 Server Install (Vultr Cloud)](https://github.com/techgneek/SOC-Automation-ELK-Stack-EDR/blob/main/Windows%20Server%202022%20Installation)
<div align="center">
  <table>
    <!-- Row 1 -->
    <tr>
      <td align="center">
        <strong>Vultr Windows Server Deployment</strong><br>
        <img width="300" alt="Screenshot 1: Vultr Deployment" src="https://github.com/user-attachments/assets/ac9939b6-60ba-41c7-b3d2-9a0511ab1d34">
      </td>
      <td align="center">
        <strong>Initial Windows Server Login via RDP</strong><br>
        <img width="300" alt="Screenshot 2: Initial Login via RDP" src="https://github.com/user-attachments/assets/37c56dbf-68ed-4ac0-b275-d42e040e3065">
      </td>
    </tr>
  </table>
</div>

- [Sysmon Installation on 2022 Windows Server](https://github.com/techgneek/SOC-Automation-ELK-Stack-EDR/blob/main/Sysmon%20Installation%20on%20Windows%20Server%202022)

<div align="center">
  <table>
    <tr>
      <td align="center">
        <strong>Sysmon Installation Command</strong><br>
        <img width="300" alt="Sysmon Installation Command" src="https://github.com/user-attachments/assets/06874827-1bd5-43f2-af4c-99dac4631161">
      </td>
      <td align="center">
        <strong>Sysmon Configuration File</strong><br>
        <img width="300" alt="Sysmon Configuration File" src="https://github.com/user-attachments/assets/113cfd78-88a4-4efe-9d09-08610e48ba40">
      </td>
      <td align="center">
        <strong>Sysmon Running in Task Manager</strong><br>
        <img width="300" alt="Sysmon Running in Task Manager" src="https://github.com/user-attachments/assets/b7e585fe-6aac-439e-8db7-d776dc9c0c68">
      </td>
      <td align="center">
        <strong>Sysmon Event Viewer Logs</strong><br>
        <img width="300" alt="Sysmon Event Viewer Logs" src="https://github.com/user-attachments/assets/582c6270-58cb-4747-8669-a2d803513bb7">
      </td>
    </tr>
  </table>
</div>

- [Elastic Agent - Fleet Server Installation](https://github.com/techgneek/SOC-Automation-ELK-Stack-EDR/blob/main/Elastic%20Agent%20-%20Fleet%20Server%20Installation)
<div align="center">
  <table>
    <!-- Row 1 -->
    <tr>
      <td align="center">
        <strong>Fleet Server Overview</strong><br>
        <img width="300" alt="Fleet Server Overview" src="https://github.com/user-attachments/assets/5b6e302f-be26-4a40-9f47-2db149c92aad">
      </td>
      <td align="center">
        <strong>Fleet Server Policy Configuration</strong><br>
        <img width="300" alt="Fleet Server Policy Configuration" src="https://github.com/user-attachments/assets/36de40dc-95c3-4b31-ad95-57b5acdef3fb">
      </td>
      <td align="center">
        <strong>Fleet Server Added</strong><br>
        <img width="300" alt="Fleet Server Added" src="https://github.com/user-attachments/assets/586d18ae-11a0-4c6a-b5f2-3eecf18f53a2">
      </td>
      <td align="center">
        <strong>Kibana Fleet Settings</strong><br>
        <img width="300" alt="Kibana Fleet Settings" src="https://github.com/user-attachments/assets/79d704a0-8164-43e2-9823-ba05f2b4a252">
      </td>
    </tr>
    <!-- Row 2 -->
    <tr>
      <td align="center">
        <strong>Windows Fleet Agent Install</strong><br>
        <img width="300" alt="Windows Fleet Agent Install" src="https://github.com/user-attachments/assets/cd29b601-2b15-4b7f-8976-81e762fdcd2c">
      </td>
      <td align="center">
        <strong>Agent Installed on Ubuntu</strong><br>
        <img width="300" alt="Agent Installed on Ubuntu" src="https://github.com/user-attachments/assets/03621103-adbc-4342-be99-a76b133c9e6e">
      </td>
      <td align="center">
        <strong>Fleet Agent Added</strong><br>
        <img width="300" alt="Fleet Agent Added" src="https://github.com/user-attachments/assets/7d7f705d-8967-47ee-a904-322ef8a94c87">
      </td>
      <td align="center">
        <strong>Fleet Agent Added to Kibana</strong><br>
        <img width="300" alt="Fleet Agent Added to Kibana" src="https://github.com/user-attachments/assets/a5c5fe4f-37e3-43c9-a4bd-47356d31e6ef">
      </td>
    </tr>
  </table>
</div>

- [Ingest Sysmon and Windows Defender Logs into Elasticsearch](https://github.com/techgneek/SOC-Automation-ELK-Stack-EDR/blob/main/Ingest%20Sysmon%20%26%20Windows%20Defender%20Logs%20Into%20Elastic)
<div align="center">
  <table>
    <!-- Row 1 -->
    <tr>
      <td align="center">
        <strong>Add Integrations</strong><br>
        <img width="300" alt="Add Integrations" src="https://github.com/user-attachments/assets/c595eb11-e9c3-409c-bf68-25cfb68fd3bd">
      </td>
      <td align="center">
        <strong>Fleet Integration Overview</strong><br>
        <img width="300" alt="Fleet Integration Overview" src="https://github.com/user-attachments/assets/4eabc9a0-45f8-40b5-a47b-a79665becbef">
      </td>
      <td align="center">
        <strong>Fleet Server Added</strong><br>
        <img width="300" alt="Fleet Server Added" src="https://github.com/user-attachments/assets/836e2168-0b92-4725-b36d-22da15bff408">
      </td>
      <td align="center">
        <strong>Custom Windows Event Logs</strong><br>
        <img width="300" alt="Custom Windows Event Logs" src="https://github.com/user-attachments/assets/facfa1f3-d38a-4092-8ade-11dda7d09b71">
      </td>
    </tr>
    <!-- Row 2 -->
    <tr>
      <td align="center">
        <strong>Windows Event Log Details</strong><br>
        <img width="300" alt="Windows Event Log Details" src="https://github.com/user-attachments/assets/c982f26c-5312-4cf6-81c1-5c08d32083a4">
      </td>
      <td align="center">
        <strong>Fleet Server Policy</strong><br>
        <img width="300" alt="Fleet Server Policy" src="https://github.com/user-attachments/assets/a47bc7c9-2b5d-4b65-a46f-3c3bb622dbe4">
      </td>
      <td align="center">
        <strong>Integration Deployed to Hosts</strong><br>
        <img width="300" alt="Integration Deployed to Hosts" src="https://github.com/user-attachments/assets/630721d1-2fea-4191-bafa-52a1e23aad5d">
      </td>
      <td align="center">
        <strong>Final Deployment</strong><br>
        <img width="300" alt="Final Deployment" src="https://github.com/user-attachments/assets/f353c590-4c8e-40d4-969d-514f3782c576">
      </td>
    </tr>
  </table>
</div>

- [SSH Server Set Up & Elastic Agent Install](https://github.com/techgneek/SOC-Automation-ELK-Stack-EDR/blob/main/Elastic%20Agent%20Install%20On%20SSH%20Server%20%26%20Log%20Authentication)
<div align="center">
  <table>
    <!-- Row 1 -->
    <tr>
      <td align="center">
        <strong>Fleet Server Overview</strong><br>
        <img width="300" alt="Fleet Server Overview" src="https://github.com/user-attachments/assets/8c5e7386-90cf-4c9e-bcd9-3c6f2d8aed3c">
      </td>
      <td align="center">
        <strong>Fleet Server Added</strong><br>
        <img width="300" alt="Fleet Server Added" src="https://github.com/user-attachments/assets/b5edcbee-fb87-4a8f-b944-a83b773a326e">
      </td>
      <td align="center">
        <strong>Kibana Fleet Settings</strong><br>
        <img width="300" alt="Kibana Fleet Settings" src="https://github.com/user-attachments/assets/57fff73d-efd3-4036-aa67-22335bcff746">
      </td>
      <td align="center">
        <strong>Elastic Agent Installation Command</strong><br>
        <img width="300" alt="Elastic Agent Installation Command" src="https://github.com/user-attachments/assets/542d04e4-052b-47de-a158-f377bd7541c5">
      </td>
    </tr>
    <!-- Row 2 -->
    <tr>
      <td align="center">
        <strong>Windows Fleet Agent Install</strong><br>
        <img width="300" alt="Windows Fleet Agent Install" src="https://github.com/user-attachments/assets/10fded8c-372d-49bf-8dff-817fa6d09868">
      </td>
      <td align="center">
        <strong>Agent Installed on Ubuntu</strong><br>
        <img width="300" alt="Agent Installed on Ubuntu" src="https://github.com/user-attachments/assets/c5837e0d-7379-4d4a-9de1-506aff3e13cb">
      </td>
      <td align="center">
        <strong>Fleet Agent Added to Kibana</strong><br>
        <img width="300" alt="Fleet Agent Added to Kibana" src="https://github.com/user-attachments/assets/3b76d4ac-ed25-4fb6-b05f-eb77b8b4fb24">
      </td>
      <td align="center">
        <strong>Fleet Logs Overview</strong><br>
        <img width="300" alt="Fleet Logs Overview" src="https://github.com/user-attachments/assets/9835e677-8669-457e-a1a2-bfcb587c01e3">
      </td>
    </tr>
  </table>
</div>

- [Alerts & Maps RDP & SSH Activity](https://github.com/techgneek/SOC-Automation-ELK-Stack-EDR/blob/main/Alerts%20%26%20Maps%20RDP%20%26%20SSH%20Activity)
<div align="center">
  <table>
    <!-- Row 1 -->
    <tr>
      <td align="center">
        <strong>SSH Failed Activity (Map)</strong><br>
        <img width="300" alt="SSH Failed Activity Query" src="https://github.com/user-attachments/assets/09bf48b5-45dc-4702-97ad-a3ba5f1522b0">
      </td>
      <td align="center">
        <strong>Creating RDP Alert</strong><br>
        <img width="300" alt="Creating SSH Rule" src="https://github.com/user-attachments/assets/45559124-c115-4991-8b86-c37a841e4359">
      </td>
      <td align="center">
        <strong>RDP Failed and Successful (Maps)</strong><br>
        <img width="300" alt="SSH Failed Authentications Map" src="https://github.com/user-attachments/assets/b9c8fd85-60c5-48e5-a1e7-68dd886e8fd2">
      </td>
      <td align="center">
        <strong>RDP Failed Activity Query</strong><br>
        <img width="300" alt="RDP Failed Activity Query" src="https://github.com/user-attachments/assets/7e63d6a7-bd9b-4e18-9b9f-7873217bb870">
      </td>
    </tr>
    <!-- Row 2 -->
    <tr>
      <td align="center">
        <strong>SSH Bruteforce Attempt Rule</strong><br>
        <img width="300" alt="Creating RDP Rule" src="https://github.com/user-attachments/assets/39811a22-f9f7-484e-9a3e-943a79cb171c">
      </td>
      <td align="center">
        <strong>SSH Failed Activity Query</strong><br>
        <img width="300" alt="RDP Failed Authentications Map" src="https://github.com/user-attachments/assets/3fae5e0d-a20e-4072-ac43-26c1d1f62fac">
      </td>
      <td align="center">
        <strong>SSH Failed and Successful Attempts (Maps)</strong><br>
        <img width="300" alt="Final Dashboard" src="https://github.com/user-attachments/assets/d1f14c2b-4b2e-4af6-9623-0bb63d54287a">
      </td>
      <td align="center">
        <strong>SSH Failed Activity Query</strong><br>
        <img width="300" alt="SSH Failed Activity Query" src="https://github.com/user-attachments/assets/d3ec7993-fb2f-4bab-9ddf-1831dc51a780">
      </td>
    </tr>
    <!-- Row 3 -->
    <tr>
      <td align="center">
        <strong>Creating SSH Alert</strong><br>
        <img width="300" alt="Creating SSH Rule" src="https://github.com/user-attachments/assets/5745d220-6c5f-434d-a764-1bd043ded295">
      </td>
      <td align="center">
        <strong>SSH Failed Activity Rule</strong><br>
        <img width="300" alt="RDP Failed Activity Query" src="https://github.com/user-attachments/assets/fdd6ca96-4f51-4286-9328-1cd2cb1f0616">
      </td>
      <td align="center">
        <strong>Creating RDP Alert</strong><br>
        <img width="300" alt="RDP Failed Authentications Map" src="https://github.com/user-attachments/assets/e02240b1-de94-4913-82ab-55291d552146">
      </td>
      <td align="center">
        <strong>Failed RDP Alert</strong><br>
        <img width="300" alt="Final Dashboard" src="https://github.com/user-attachments/assets/2ba3466e-cbbb-4843-81a5-1e5548d69ea5">
      </td>
    </tr>
  </table>
</div>

- [Mythic Server Installation](https://github.com/techgneek/SOC-Automation-ELK-Stack-EDR/blob/main/Mythic%20Server%20Installation)
  
  <div align="center">
  <table>
    <!-- Row 1 -->
    <tr>
      <td align="center">
        <strong>Mythic Firewall Group</strong><br>
        <img width="300" alt="Docker Install Command" src="https://github.com/user-attachments/assets/044687e7-6be7-4c22-a531-18194af6d412">
      </td>
      <td align="center">
        <strong>Cloning Mythic Repository</strong><br>
        <img width="300" alt="Cloning Mythic Repository" src="https://github.com/user-attachments/assets/5cee4461-0f1c-42cd-a3b5-864241451022">
      </td>
      <td align="center">
        <strong>Starting Mythic Services</strong><br>
        <img width="300" alt="Starting Mythic Services" src="https://github.com/user-attachments/assets/d5bbb30a-bdd4-4df9-be70-e02299eb43bf">
      </td>
    </tr>
    <!-- Row 2 -->
    <tr>
      <td align="center">
        <strong>Retrieving Mythic Password</strong><br>
        <img width="300" alt="Retrieving Mythic Password" src="https://github.com/user-attachments/assets/749b1bc3-31a1-4a2c-9afa-5b569007ad40">
      </td>
      <td align="center">
        <strong>Mythic Server Port Listening</strong><br>
        <img width="300" alt="Mythic Web GUI Login" src="https://github.com/user-attachments/assets/c1a1fbd7-6f77-4b3b-beff-82750f42ac6e">
      </td>
      <td align="center">
        <strong>Mythic Server Deployment On Vultr Clound</strong><br>
        <img width="300" alt="Mythic Web GUI Overview" src="https://github.com/user-attachments/assets/25398f66-33e6-41a4-85cd-b564971643e1">
      </td>
    </tr>
  </table>
</div>

- [Mythic Server and Agent Setup (C2 Framework)](https://github.com/techgneek/SOC-Automation-ELK-Stack-EDR/blob/main/Mythic%20Server%20and%20Agent%20Setup)
<div align="center">
  <table>
    <!-- Row 1 -->
    <tr>
      <td align="center">
        <strong>Mythic Web GUI Login</strong><br>
        <img width="300" alt="Mythic Web GUI Login" src="https://github.com/user-attachments/assets/b2f4d747-26f9-4d27-b753-e1e2f97b0b0f">
      </td>
      <td align="center">
        <strong>Mythic Callback Interface</strong><br>
        <img width="300" alt="Mythic Callback Interface" src="https://github.com/user-attachments/assets/fe45af7f-1ae4-4b96-b8cf-41b25ef3135a">
      </td>
      <td align="center">
        <strong>Payload Configuration Overview</strong><br>
        <img width="300" alt="Payload Configuration Overview" src="https://github.com/user-attachments/assets/012f8d6a-093e-46ce-8277-f6d9a4d37d27">
      </td>
      <td align="center">
        <strong>Wordlist Preparation in Kali Linux</strong><br>
        <img width="300" alt="Wordlist Preparation in Kali Linux" src="https://github.com/user-attachments/assets/3cebf6e8-1b55-446f-8933-7378aefa6146">
      </td>
      <td align="center">
        <strong>RDP Brute Force Attack</strong><br>
        <img width="300" alt="RDP Brute Force Attack" src="https://github.com/user-attachments/assets/288bd21e-6428-40aa-9652-0481204be1d7">
      </td>
    </tr>
    <!-- Row 2 -->
    <tr>
      <td align="center">
        <strong>Accessing Windows Server</strong><br>
        <img width="300" alt="Accessing Windows Server" src="https://github.com/user-attachments/assets/6133d6a0-5e31-4c39-8da2-fe7b545c3853">
      </td>
      <td align="center">
        <strong>Password File Creation</strong><br>
        <img width="300" alt="Password File Creation" src="https://github.com/user-attachments/assets/05800a7c-5ba1-4af4-b13c-c32ad0f38385">
      </td>
      <td align="center">
        <strong>Windows Defender Disabled</strong><br>
        <img width="300" alt="Windows Defender Disabled" src="https://github.com/user-attachments/assets/6e599524-e6d8-4cc6-aee8-8a0b80ff2565">
      </td>
      <td align="center">
        <strong>File Download Using Mythic</strong><br>
        <img width="300" alt="File Download Using Mythic" src="https://github.com/user-attachments/assets/92610211-cc68-4625-b978-cd6b6c253f07">
      </td>
      <td align="center">
        <strong>Final Payload Execution</strong><br>
        <img width="300" alt="Final Payload Execution" src="https://github.com/user-attachments/assets/e7981ac8-fcd0-480f-9447-3962f35a9037">
      </td>
    </tr>
  </table>
</div>

- [Mythic C2 - Alerts and Dashboard](https://github.com/techgneek/SOC-Automation-ELK-Stack-EDR/blob/main/Mythic%20C2%20-%20Alerts%20and%20Dashboard)
  
<div align="center">
  <table>
    <!-- Row 1 -->
    <tr>
      <td align="center">
        <strong>Network Connections Visualization</strong><br>
        <img width="300" alt="Network Connections Visualization" src="https://github.com/user-attachments/assets/5637c510-e723-4734-be7d-fe6159be8a2a">
      </td>
      <td align="center">
        <strong>External Network Connections</strong><br>
        <img width="300" alt="External Network Connections" src="https://github.com/user-attachments/assets/3cf1add8-06f0-4d23-a5b6-952d7dd15588">
      </td>
      <td align="center">
        <strong>Suspicious Activity Dashboard</strong><br>
        <img width="300" alt="Suspicious Activity Dashboard" src="https://github.com/user-attachments/assets/7c00758a-7dd5-4f0a-8537-2e69c9f9d971">
      </td>
      <td align="center">
        <strong>Process Create Events</strong><br>
        <img width="300" alt="Process Create Events" src="https://github.com/user-attachments/assets/f4f3d83f-ed2f-46fe-860b-89e72c1a8646">
      </td>
      <td align="center">
        <strong>Alert Rule for Process Create</strong><br>
        <img width="300" alt="Alert Rule for Process Create" src="https://github.com/user-attachments/assets/cdf7fbeb-700a-48f2-8393-14f9275c9f3a">
      </td>
    </tr>
    <!-- Row 2 -->
    <tr>
      <td align="center">
        <strong>Detection Rule in Kibana</strong><br>
        <img width="300" alt="Detection Rule in Kibana" src="https://github.com/user-attachments/assets/b4dcedf7-5628-4f0e-9bca-0a2716cd392f">
      </td>
      <td align="center">
        <strong>Event ID 1: Process Creates</strong><br>
        <img width="300" alt="Event ID 1 Process Creates" src="https://github.com/user-attachments/assets/2de4d1f9-c32c-4a18-ac65-469fc89fc324">
      </td>
      <td align="center">
        <strong>SHA256 Analysis</strong><br>
        <img width="300" alt="SHA256 Analysis" src="https://github.com/user-attachments/assets/4e89bd1c-2016-4ada-aaeb-38da815a6262">
      </td>
      <td align="center">
        <strong>Elastic Query Results</strong><br>
        <img width="300" alt="Elastic Query Results" src="https://github.com/user-attachments/assets/5cace8d9-d8b3-4af1-a9a0-91fbcbea8731">
      </td>
      <td align="center">
        <strong>TechGneek-Suspicious-Activity Dashboard</strong><br>
        <img width="300" alt="TechGneek-Suspicious-Activity Dashboard" src="https://github.com/user-attachments/assets/4e3daab5-648c-4a20-b206-89fd92144d74">
      </td>
    </tr>
  </table>
</div>

- [osTicket Setup & Configuration](https://github.com/techgneek/SOC-Automation-ELK-Stack-EDR/blob/main/osTicket%20Setup%20%26%20Configuration)

<div align="center">
  <table>
    <!-- Row 1 -->
    <tr>
      <td align="center">
        <strong>Downloading XAMPP for osTicket Config</strong><br>
        <img width="300" alt="Downloading osTicket" src="https://github.com/user-attachments/assets/babba31f-b078-49fb-8612-5809afec272c">
      </td>
      <td align="center">
        <strong>Configuring XAMPP</strong><br>
        <img width="300" alt="Configuring XAMPP" src="https://github.com/user-attachments/assets/a4840f44-65f2-4472-96d6-0a6d8e3e1e0d">
      </td>
      <td align="center">
        <strong>Editing phpMyAdmin Configuration</strong><br>
        <img width="300" alt="Editing phpMyAdmin Configuration" src="https://github.com/user-attachments/assets/7484620d-55c6-4313-897d-ccb0fcc159c6">
      </td>
    </tr>
    <!-- Row 2 -->
    <tr>
      <td align="center">
        <strong>Firewall Configuration</strong><br>
        <img width="300" alt="Firewall Configuration" src="https://github.com/user-attachments/assets/bca1580c-761b-48b0-9d09-b39564a11d4f">
      </td>
      <td align="center">
        <strong>phpMyAdmin Database Setup</strong><br>
        <img width="300" alt="phpMyAdmin Database Setup" src="https://github.com/user-attachments/assets/20105baf-b7a7-4e57-9046-d63d58ccd726">
      </td>
      <td align="center">
        <strong>osTicket Initial Setup</strong><br>
        <img width="300" alt="osTicket Initial Setup" src="https://github.com/user-attachments/assets/72710660-78d0-4f08-be71-dde1dfe56a3b">
      </td>
    </tr>
    <!-- Row 3 -->
    <tr>
      <td align="center">
        <strong>Renaming Configuration File</strong><br>
        <img width="300" alt="Renaming Configuration File" src="https://github.com/user-attachments/assets/9fa1b853-18a1-41ea-aa57-19ec928643bc">
      </td>
      <td align="center">
        <strong>osTicket Installation Completed</strong><br>
        <img width="300" alt="osTicket Installation Completed" src="https://github.com/user-attachments/assets/7e9b6423-8c88-4e5a-adaa-1b16f38f8678">
      </td>
      <td align="center">
        <strong>Final osTicket Dashboard</strong><br>
        <img width="300" alt="Final osTicket Dashboard" src="https://github.com/user-attachments/assets/35b65f75-bb69-4dca-96c5-85b24c0dd653">
      </td>
    </tr>
  </table>
</div>

- [osTicket & ELK Stack Integration](https://github.com/techgneek/SOC-Automation-ELK-Stack-EDR/blob/main/osTicket%20%26%20ELK%20Stack%20Integration)

<div align="center">
  <table>
    <!-- Row 1 -->
    <tr>
      <td align="center">
        <strong>Successful Webhook Test</strong><br>
        <img width="300" alt="Successful Webhook Test" src="https://github.com/user-attachments/assets/10c3a9cf-44ef-484a-8308-1a518b8c2887">
      </td>
      <td align="center">
        <strong>Private IP Configuration</strong><br>
        <img width="300" alt="Private IP Configuration" src="https://github.com/user-attachments/assets/fc4961b7-c6ae-4cf1-8749-46ec5ad9c176">
      </td>
      <td align="center">
        <strong>Ping Test Results</strong><br>
        <img width="300" alt="Ping Test Results" src="https://github.com/user-attachments/assets/75c9c1dd-10fa-493f-ac18-8540342f3767">
      </td>
      <td align="center">
        <strong>Overview of Completed Steps</strong><br>
        <img width="300" alt="Overview of Completed Steps" src="https://github.com/user-attachments/assets/6549e86f-c205-4acd-b08d-e984e12e4d6b">
      </td>
    </tr>
    <!-- Row 2 -->
    <tr>
      <td align="center">
        <strong>osTicket Logs</strong><br>
        <img width="300" alt="osTicket Logs" src="https://github.com/user-attachments/assets/a679bfa0-30f9-4cbd-b714-a7e07218403b">
      </td>
      <td align="center">
        <strong>osTicket API Key</strong><br>
        <img width="300" alt="osTicket API Key" src="https://github.com/user-attachments/assets/3af757a3-05e9-4607-b018-44ed7284e97d">
      </td>
      <td align="center">
        <strong>Failed Webhook Test</strong><br>
        <img width="300" alt="Failed Webhook Test" src="https://github.com/user-attachments/assets/688bc4da-44b7-4c1c-b439-5fe262acfde6">
      </td>
      <td align="center">
        <strong>Confirmed Successful IP Configuration</strong><br>
        <img width="300" alt="Confirmed Successful IP Configuration" src="https://github.com/user-attachments/assets/b0006705-0fa1-492c-9c74-83c875a79592">
      </td>
    </tr>
  </table>
</div>








