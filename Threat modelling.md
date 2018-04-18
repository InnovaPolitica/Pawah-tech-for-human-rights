## Threat modelling

We based our Threat modelling in the SANS Institute (2005) and the Microsoft model. 

Pawah! is based in the security triad: Confidentiality, integrity, and availability. It seeks to protect the records of human rights violations so they can be used in trials and investigations. It also protects the witness through a fake front-end that reinforces plausible deniability. It  encrypts the information and guarantees that the information captured by your mobile is the same saved in the secured server, and shows that the information has not been edited or manipulated. The information would be saved in a secured cloud so it can be access later. 

## Assets identified: 
We have identified as main assets that we want to protect with Pawah the following:
- Physical safety of activists, human rights defenders, journalists and citizens. 
- Opportunity of victims of human rights abuses to access to auditable and reliable evidence to claim for justice (transitional justice) 
- Confidential records of human rights abuse (Stored in the devices and the secured cloud) 
- Storage in the secured cloud
- Plausible deniability of activists (We understand it as the ability the possibility to deny knowledge of or responsibility for any damnable actions).
- Available storage space. It is important to have enough available space to storage all the information.

## Trust boundaries: 
We identified two trust boundaries within the use of Pawah. The level 1, is between the user and the app, this involves only the records taken with the app but that have not been uploaded yet (they remain in the memory of the device but hidden and encrypted). The level 2, involves the records when they have been encrypted and saved in the blockchain (see diagram below).

## Entry points: 
Potential entry points are: the user's own device (through device seizure, spoofing, repudiation, elevation of privilege). 

## Architecture overview: 
- Use scenario. A fake front-end to create video and audio records of human rights abuses through photographs, photographs, videos or audio. Use of records for legal purposes and journalistic investigation.
- External dependency. Actions of violent repression/physical attack, intimidation, kidnapping and imprisonment against activists, human right defenders, journalists, citizens.  
- Internal security risks. Potential device seizures, monitoring of devices, security breaches.    

## Modeling the system. We model the system in this diagram

### Diagram 1. Main architecture of Pawah!



## Threats identified
A threat is understand as  new or newly discovered incident with the potential to do harm to the system or the organization.

### -Unintentional: 
It is possible that users can give unintentional access to their accounts because of lost devices, bad administration of passwords, or social engineering. We can overload the storage space very easily, therefore it is necessary to have enough storage space and protocols to eliminate not useful information. 
### -Intentional: 
There are several intentional threats such as security forces or people implicated on human right abuses who want to get access to the devices or the cloud to erase some records, former employees or competitors who want the system to collapse or get errors, authoritative governments that feel that this tool is against their interests and prohibit its use or asks for access to the information. 
Some specific threats that we identified are: violent repression or intimidation to users so they give access to their devices, device seizures which could give limited access to the device´s memories, hacking to the network and devices and DDoS attacks, Brute force attacks against the credential store.
Flooding the storage space with useless information to affect the server.  

## Vulnerabilities
Vulnerabilities are known weakness that can be exploited to attack the system. 

Some vulnerabilities identified are potential software bugs that can affect the functionality of Pawah!, broken processes that might corrupt files or affect them in anyhow and hardware problems to run Pawah!.
Credential steel. They can be stolen from either the credential store or the network. We will have a passcode to access the app/the information and we will have web access to the secure cloud storage. If the credentials are stolen and an attacker can get in you lose everything as the proofs can now be viewed and maybe deleted. The attackers can change the passcode and lock the legitimate user out. For that reason, it is important to use a strong hashing algorithm to access the cloud where details are stored. 

## Risks
Risks are potential for loss or damage when a threat exploits a vulnerability. We can say, they are the result of threats and vulnerabilities combined. 

The most important risks that Pawah! has are: losing confidence of users because of hacked information, being unable to proof the authenticity of the records saved through Pawah! and all the information being compromised. 

## STRIDE analysis:
        In our STRIDE analysis we identified the following potential threats:
### Spoofing: 
Impersonation can happen when someone intents to modify or corrupt one of the records taken with Pawah! using a registered and verified user account. Normally this happens because of social engineering, phishing or other tactic. In order to neutralize this threat we are going to implement blockchain so integrity of information can be guarantee along the process even if there is impersonation. 

### Tampering: 
This form of falsification of data could normally happen when  the records are in the user's own device or between the connection with the network carrier or within the Wifi network. For this we will use a double encryption: the first one would be asymmetric within the own device once the record has being saved and the second (asymmetric), when the file is transfered to the blockchain.

### Repudiation: 
Can happen if malicious users can try to misuse Pawah! or manipulate it in anyhow. For this, we want to integrate Pawah! with Keybase as a way to have strong authentication of users. 
### Information Disclosure: 
Even though the registries and logs of the files are going to be available to the scrutiny of everybody through blockchain, identity and the contents would remain encrypted.
### Denial of Service: 
In centralized clouds this kind of attacks can result very successful. Nevertheless, companies such as Gladius are proving that in the blockchain infrastructure, DDoS attacks are less effective. 
### Elevation of privilege. 
Could happen if an unprivileged user gains privileged access to compromise or destroy the entire system. For this, we will work in a strong policy and security protocols.

## Governance
Pawah! is a tool that is being created with the support of several activists and organizations involved in the defense of human rights. The development of the tool and the management of its assets will be in hands in Asuntos del Sur and its project of Political Innovation. Nevertheless, any decision that could affect the functioning of the app and the personal data stored in the secured cloud will be taken after consulting the users and the organizations involved. 

## Regulation
Coming soon, we will be doing an exploratory analysis of international and national laws that could affect the functionality of Pawah! Please, if you have some knowledge of the current regulation, help us and contribute! 
