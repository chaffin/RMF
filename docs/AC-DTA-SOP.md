---
title: Data Transfer Agent SOP
---

# 1.  PURPOSE
   The purpose of this Standard Operating Procedure (SOP) is to provide processes and procedures under the security control (AC-4) Information Flow Enforcement when conducting low risk Assure File Transfer (AFT) in accordance with Reference (a) for the ([Information System]). 

# 2.  REFERENCES
  a.  ARMY Assured File Transfer Guide, July 2015<br>
  b.  Joint Special Access Program (SAP) Implementation Guide (JSIG), April 2016<br>
  c.  JSIG-Rev.4 Based Army SAP/SA System Security Plan (SSP)<br>
  d.  US Army CIO-G6 Special Programs Office, Assured File Transfer Training for Low Risk Data Transfers, November 2013. 

# 3.  SCOPE  
   This SOP enforces approved authorizations in controlling the flow of information within the [Information System] system. The [Information System] utilizes mandatory and discretionary access controls for all file types based on the concept of least privilege and by the separation of duties, which are enforced by local and domain policies. When data are extracted from the information system, information flow enforcement is maintained utilizing the AFT process and role-based Data Transfer Agent (DTA) scheme as described within this SOP.

# 4.  RESPONSIBILITIES
   Key roles and responsibilities are outlined in Reference (c). The below duties are specific under this SOP for the AFT process.

a. Program Security Officer (PSO)
  
   Government official responsible for appointing the Data Transfer Agent (DTA) for low risk data transfer.

b. Contractor Program Security Officer (CPSO)
   1. Contractor providing security control measures for the accountability and marking digital media under this SOP.
   2. Responsible for appointing a TPI Media Custodian in writing.
   3. Ensures Data Transfer Agents (DTA) receive training in low risk Assured File Transfers.
   4. Authorizes each AFT by signing DTA request form [Appendix A](#appendix-a) as the approver.

c. Information System Security Manager (ISSM)
   1. Government official responsible for appointing the ISSO and updating Reference (c).  
   2. Proponent of this SOP and conducts periodic compliance inspections.

d. Information System Security Officer (ISSO)  
   1. Contractor providing direct support to the program.
   2. Appointed by the ISSM to conduct privilege audit administration functions.
   3. Conducts weekly audits to include all AFT actions, comparing technical audit trails with the media custodian’s media log.
   4. Conducts weekly audits of the DTA roles, ensuring they are only active when required.

e. System Administrator (SA)
   1. Contractor providing direct support to the program.
   2. Maintains the administration functions and responsible for activating/deactivating the DTA role within the [Information System].

f. Data Transfer Agent (DTA)  
   1. Contractor providing direct support to the program.  
   2. An [Information System] user authorized and trained in a privileged role to conduct assured file transfers.  
   3. Conducts low risk Assured File Transfers and ensures data is appropriately handled per section (5.j) and signs the DTA request form [Appendix A](#appendix-a) as the DTA.

g. Two Person Integrity (TPI) Media Custodian  
   1. Contractor providing direct support to the program.  
   2. Appointed in writing by the CPSO.  
   3. Maintains the TPI Log to reflect accountability of removable media throughout the [Information System] life cycle; from receipt of the media to destruction or the media. 

h. Requestor
  
   Initiates DTA process by completing the DTA request form [Appendix A](#appendix-a), signing the form as the requestor and routing it for approval.

i. Witness

   Signs the DTA request form [Appendix A](#appendix-a) as the witness.  The witness cannot be any personnel performing an active in the immediate file transfer being conducted role (i.e. the SA that initiated the DTA rights, the requestor for this transfer, the TPI custodian, the approver, and/or the DTA conducting the transfer).

# 5. PROCEDURES
  
   The below procedures satisfy several controls from Reference (c) and are specific to the [Information System] to ensure information flow enforcement when conducting AFT. 

a. File Types
  
   There are no file type restrictions under this SOP.  

b. Media Use (RMF Control MP-2)
   1. The use of removable media is restricted on the [Information System].  CDs and DVDs are the only media type authorized for use under this SOP for AFT.  
   2. The following type of digital media are prohibited and not authorized for AFTs include, but not limited to, hard disks, floppy disks, zip drives, thumb drives, pen drives, flash drives, and similar universal serial bus (USB) storage devices.  
   3. Access to removable media writing capabilities is not authorized by users of the [Information System] to include privileged and general users with the exception of trained Data Transfer Agents approved for temporary elevated privileges under this SOP.  
   4. All portable media transferred under this SOP shall be protected with encryption using the open source software 7-Zip and transported and moved in accordance with (5.i.2).  
   5. All digital media and the use of such media on the [Information System] are accountable.  All digital media shall be authorized by the CPSO prior to being introduced into the [Information System] as described in (5.i.3).  
   6. User roles and access privileges are outlined in the [Information System] SSP Reference (c) Section (8.4).  
   7. Personally-owned media as well as media listed in (5.b.2) are prohibited for use on the [Information System] and are not approved for AFT.  

c. Role Based Schemes (RMF Control AC-2(7))  
   1. The transferring of data is a privileged action conducted by the Data Transfer Agent (DTA) role.  
   2. The [Information System] is configured with a DTA GroupPolicy that when enabled by the System Administrator (SA) role via security group assignment, authorizes write access to the DTA role.  
   3. The DTA role is monitored and audited by the Information System Security Officer (ISSO) role.  
   4. The TPI Media Custodian role maintains accountability for the removable media before and after each AFT.  

d. Dual Authorization (RMF Control AC-3(2))  
   1. Only appointed and trained Data Transfer Agents are authorized to transfer data from the [Information System] to removable media.  
   2. The [Information System] SA is the only role authorized to enable permissions to allow the DTA write access to removable media.  
   3. The ISSO and SA shall receive notification from the CPSO when the DTA role is to be activated. The method of notification must provide an auditable trail.  
      1. a. Upon notification the SA will ensure the DTA user is logged off all [Information System] systems.  
      2. b. The SA will move the DTA from the restricted user security group to the DTA security group and have the user log into a [Information System] workstation.  
      3. c. The SA will verify the ability to burn disc is granted.  
      4. d. Upon completion of the AFT by the DTA, the SA shall ensure the DTA is logged off all [Information System] systems.  
      5. e. The SA will move the DTA from the DTA security group to the restricted user group and have the user log into a [Information System] workstation.  
      6. f. The SA will verify the ability to burn disc is removed.  

e. Separation of Duties (RMF Control AC-5)  
   1. The separation of duties for the ISSO, SA, DTA, and TPI Media Custodian under this SOP are incorporated in the [Information System] GroupPolicy roles as outlined below:  
      1. a. The SA, ISSO, TPI Media Custodian and the DTA shall not be the same individual.  
      2. b. The SA shall not perform security audit functions.  
      3. c. The ISSO shall not perform SA functions.  

>> f.  Least Privilege: Authorized Access to Security Functions (RMF Control AC-6(1))  
>>> 1.  The concept of least privilege is employed under this SOP by limiting write access to removable media to appointed DTAs trained in the AFT process via technical controls.  
>>> 2.  The use of role-based schemes in (5.c) enforces the most restrictive access to removable media by temporarily allowing the DTA write access to removable media to conduct AFT without maintaining a separate privileged account.  
>>> 3.  Blanket approvals and extended periods of authorized access to the DTA role are not authorized under this SOP.  

>> g.  Information Flow Enforcement (RMF Control AC-4)  
>>> 1.  The flow of information for AFT is tracked throughout the [Information System] life cycle as follows:  
  >>>> a.  The DTA will be issued, factory fresh, accountable removable media from the TPI custodian.  
  >>>> b.  The CPSO will notify the ISSO and SA per (5.d.3).  
  >>>> c.  The DTA will conduct the low risk AFT and return the media to the TPI custodian and update the TPI media log per (5.g.3) and proceed with storage, dissemination, and or destruction.  

>>> 2.  The TPI media log shall remain unclassified and not contain classified file names or information.

>>> 3.  The TPI media custodian shall ensure the following information is recorded in the TPI log:
  >>>> a.  Date – Date of the AFT;  
  >>>> b.  DTA – Name of the user conducting the AFT;  
  >>>> c.  File Names – Formatted as [YYYYMMDD_XX] (i.e., 20101225_01).   
  >>>> d.  Source – The system source the files are transferred. (e.g., [Information System]);  
  >>>> e.  Destination – Where the files will be transferred to. (e.g., Government, ASEP).  

>>> 4.  The media shall be marked and protected in accordance with the Security Classification Guide and handled in accordance with the facility’s document control processes and procedures.  

>> h.  Role Based Security Training (RMF Control AT-3)
>>> 1.  The CPSO shall ensure all users receive initial and annual General and Privilege User training to include the review of this SOP.  
>>> 2.  The CPSO shall ensure users assigned to the DTA role are trained in accordance with References (a) and (d).  

>> i.  Protection of Information at Rest: Cryptographic Protection (RMF Control SC-28(1))  
>>> 1.  To protect the confidentiality and integrity of information transferred to and stored on removable media the [Information System] implements DoD/NSA approved cryptographic mechanisms to prevent unauthorized disclosure and modification of data at rest, CDs and other removable media (e.g., DVDs) by following the Data Transfer process in (5.j).  
>>> 2.  The transport and movement of all media is restricted to an authorized custodian by means of a courier card/letter, which are outside the scope of this SOP, and shall be coordinated through the CPSO for approved procedures.  
>>> 3.  Before introducing media to the [Information System], the media must be accountable and handled in accordance with the facility’s document control processes and procedures.  

>> j.  Data Transfer  
>>> 1.  The DTA will ensure the data files being transferred are consolidated within a single top level folder and follow the below steps to encrypt and transfer to removable media.  
>>> 2.  Using the mouse, hover over the top level folder and ```[RIGHT]``` click, then select ```[7-ZIP]``` from the menu option.  
>>> 3.  Select ```[ADD TO ARCHIVE]``` and follow the below method to name the archive.  
  >>>> a.  AFT File names shall be formatted per (5.g.3.a).  
    >>>>> Note: File extensions such as .zip, .7z are assumed in AFT archived filenames and need not be recorded in the media log.  
  >>>> b.  Sequential AFT archives on the same date will increment in the suffix.  

>>> 4.  The DTA shall type the approved known access code in the password area under ```[ENTER PASSWORD]``` and ```[REENTER PASSWORD]``` blocks.  
  >>>> a.  The approved known access code used for conducting AFT is not considered an authenticator, rather an access code and shall be protected similar a GSA approved container or combination lock.  
    >>>>> Note: The access code for AFTs shall be a coordinated effort between the PSO and CPSO and may have an indefinite expiration date.  
  >>>> b.  The access code shall be known by all who have need-to-know and only changed when directed by the PSO.  

>>> 5.  After entering the access code, the DTA will check the ```[ENCRYPT FILE NAMES]``` box and select ```[OK]```. Doing this encrypts the folder.  

>>> 6.  The DTA shall test the archive by following the below steps:  
  >>>> a.  Open the 7-Zip File Manager.  
  >>>> b.  Within the 7-Zip File Manager, navigate to the encrypted file location.  
  >>>> c.  Double click on the encrypted file to open;  
  >>>> d.  7-Zip should challenge by requesting the access code;  
  >>>> e.  Enter the code/password, and verify that it works.  
  >>>>> IF 7-Zip does not challenge for an access code, or the access code does not work, immediately stop the process. Do not transfer the archive to media and return to (5.j.1).  

>>> 7.  The DTA shall now burn the protected file archive to the removable media issued by the TPI Media Custodian by following the below steps:  
  >>>> a.  Navigate to the encrypted file and ```[RIGHT]``` click to open the menu options.    
  >>>> b.  Select ```[SEND TO]``` and chose the DVD RW Drive.  
  >>>> c.  Select ```[WITH A CD/DVD PLAYER]``` and click ```[NEXT]```.  
  >>>> d.  Click ```[BURN TO DISC]``` on the top bar, select ```[NEXT]``` and then select ```[FINISH]``` when prompted.

>>> 8.  Once the burn is complete, reinsert the disc and attempt to open the file using the 7-Zip File Manager program.
  >>>> a.  Click on the small, drop down arrow on the top, right hand side of the window, select “D:” and open the file by entering the password.  
>>>>> i.  The media fails to open, the DTA shall return the media to the TPI media custodian per (5.g.1.c) and attempt the process over. <br>
>>>>> ii.  The media transferred successfully, the DTA shall immediately return the media to the TPI media custodian per (5.g.1.c) and ensure the DTA role is deactivated per (5.d.3.b).

# Appendix A


