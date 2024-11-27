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
    </tr>
  </table>
</div>








