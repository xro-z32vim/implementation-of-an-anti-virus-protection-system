# implementation-of-an-anti-virus-protection-system

    We will study the process of implementing information security solutions. In the material:      
    You will understand what data is needed to determine the optimal deployment scenario for the implemented system.     
    Get acquainted with the requirements for the implemented system.

# Deploying a solution, setting a task

In order to approach the topic of the pre-project survey and inventory with a new understanding, we propose to formulate the task statement. In large projects, the requirements for the implemented system form the basis of the terms of reference. This is one of the most important design documents, on the basis of which a technical solution is drawn up describing the architecture and functioning of the system, and a test program, based on the results of which a decision will be made on the possibility of putting the system into operation.
What is needed to implement the project:

    It is required to implement an antivirus protection system as part of:
    management servers;
    workstation protection module;
    the server protection module.
    All assets must be included in the Active Directory domain.
    The management server must be running Microsoft Windows Server OC.
    The management server's service information must be stored on a dedicated server with a PostgreSQL database management system.
    The management server must scan the specified network ranges and domain for new hosts.
    Antivirus protection software should be distributed centrally from the management server to PCs and servers that are located in administrative groups according to the asset type.
    Antivirus databases, modules, and software should be updated automatically on a schedule.
    A policy of blocking selected categories of applications should be implemented for the PC.
    Critical events from connected devices should be stored in the event log of the management server.
    The management server should be able to connect a technical support specialist with rights to view asset information and connect to a remote desktop. Management rights are not granted.
    Critical events should be sent to SIEM to monitor information security events in this infrastructure.
