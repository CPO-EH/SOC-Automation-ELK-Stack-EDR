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


