# LotCoM

### Status
<div align=left>
  <table>
    <tr>
      <th></th>
      <th>Printer Application</th>
      <th>Client Application</th>
      <th>Scanner Scripts</th>
      <th>Watcher Service/Script</th>
    </tr>
    <tr>
      <td>Release Status</td>
      <td>
        <img src="https://img.shields.io/github/actions/workflow/status/LotCoM/LotCoM-printer/cicd.yml?branch=stable&style=for-the-badge&label=.NET%20CI%2FCD"/>
        <img src="https://img.shields.io/github/actions/workflow/status/LotCoM/LotCoM-printer/github-code-scanning%2Fcodeql?style=for-the-badge&label=CodeQL"/>
      </td>
      <td>
        <img src="https://img.shields.io/github/actions/workflow/status/LotCoM/LotCoM-client/github-code-scanning%2Fcodeql?style=for-the-badge&label=CodeQL"/>
      </td>
      <td>
        <img src="https://img.shields.io/github/actions/workflow/status/LotCoM/LotCoM-scanner-configs/github-code-scanning%2Fcodeql?style=for-the-badge&label=CodeQL"/>
      </td>
      <td>
        <img src="https://img.shields.io/github/actions/workflow/status/LotCoM/LotCoM-watcher/github-code-scanning%2Fcodeql?style=for-the-badge&label=CodeQL"/>
      </td>
    </td>
    <tr>
      <td>Monthly Commits</td>
       <td>
          <img src="https://img.shields.io/github/commit-activity/m/LotCoM/LotCoM-printer?authorFilter=masonritchason&style=for-the-badge&label=Commits"/>
       </td>
       <td>
          <img src="https://img.shields.io/github/commit-activity/m/LotCoM/LotCoM-client?authorFilter=masonritchason&style=for-the-badge&label=Commits"/>
       </td>
       <td>
          <img src="https://img.shields.io/github/commit-activity/m/LotCoM/LotCoM-scanner-configs?authorFilter=masonritchason&style=for-the-badge&label=Commits"/>
       </td>
       <td>
          <img src="https://img.shields.io/github/commit-activity/m/LotCoM/LotCoM-watcher?authorFilter=masonritchason&style=for-the-badge&label=Commits"/>
       </td>
    </tr>
    <tr>
      <td>Languages</td>
       <td>
          <img src="https://img.shields.io/github/languages/count/LotCoM/LotCoM-printer?style=for-the-badge"/>
       </td>
       <td>
          <img src="https://img.shields.io/github/languages/count/LotCoM/LotCoM-client?style=for-the-badge"/>
       </td>
       <td>
          <img src="https://img.shields.io/github/languages/count/LotCoM/LotCoM-scanner-configs?style=for-the-badge"/>
       </td>
       <td>
          <img src="https://img.shields.io/github/languages/count/LotCoM/LotCoM-watcher?style=for-the-badge"/>
       </td>
    </tr>
    <tr>
      <td>Top Language</td>
       <td>
          <img src="https://img.shields.io/github/languages/top/LotCoM/LotCoM-printer?style=for-the-badge"/>
       </td>
       <td>
          <img src="https://img.shields.io/github/languages/top/LotCoM/LotCoM-client?style=for-the-badge"/>
       </td>
       <td>
          <img src="https://img.shields.io/github/languages/top/LotCoM/LotCoM-scanner-configs?style=for-the-badge"/>
       </td>
       <td>
          <img src="https://img.shields.io/github/languages/top/LotCoM/LotCoM-watcher?style=for-the-badge"/>
       </td>
    </tr>
 </table>
</div>

### ERP System for Lot Data tracking at Yamada North America, Inc.
#### Developed by Mason Ritchason ([@masonritchason](https://github.com/masonritchason)).

LotCoM is a new ERP system that enables digital lot-tracing at YNA. With LotCoM, YNA is able to store and interact with lot-tracing data from every in-house production process. Starting at the raw material stage, LotCoM creates long-form chains of data that trace information from each process station. Lot-tracing data can be viewed, extracted, and manipulated to assist in part problem management. LotCoM eliminates costly paper records, allows timely lot-tracing, and cuts back on problematic human error.

LotCoM is a 3-part [Distributed System](https://stackoverflow.com/questions/72763123/what-is-meant-by-distributed-system)* that consists of the **LotCoM Client** and **LotCoM Printer** applications, and the **LotCoM Watcher** service.

### LotCoM Client (Application)
A feature-rich application that provides a window into the LotCoM database. Allows associates to view, manage, and manipulate lot-tracing data in many ways. Using fast, configurable search algorithms, users can quickly and easily find problem part ranges. With the built-in reporting tools, users can export organized, limited datasets that can be used in a wide range of applications. Manipulating, scrapping, and deleting lot-trace information is easy with LotCoM Client's intuituve Label Recreation function.

### LotCoM Printer (Application)
Low-level, high-security printing software used to produce lot-tracing labels. These labels are applied to in-house, in-process parts.

### LotCoM Watcher (Service)
WinService-style program that processes scan results from YNA's fleet of production floor handheld scanners. Reads, formats, processes, and inserts new Label scans into the LotCoM database.
