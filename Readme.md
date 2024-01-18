
**Write a list of Linux commands to do the following:
Download MongoDB zip or gzip file from here:
https://www.mongodb.com/try/download/community
(https://www.mongodb.com/try/download/community)
Extract it to the local folder. You decide the location of your folder, i.e.
/Users/v111233/Downloads/mongodbCreate a variable named $MONGO_HOME
which points to that local folder.**
0 words 

```bash
# Set the download URL to a variable
MONGODB_DOWNLOAD_URL="https://fastdl.mongodb.org/linux/mongodb-linux-x86_64-ubuntu2004-4.4.0.tgz"

# Set the local folder path
LOCAL_FOLDER="/Users/v111233/Downloads/mongodb"

# Download MongoDB zip or gzip file
wget "$MONGODB_DOWNLOAD_URL" -O mongodb.tgz

# Create the local folder if it doesn't exist
mkdir -p "$LOCAL_FOLDER"

# Extract the downloaded file to the local folder
tar -zxvf mongodb.tgz -C "$LOCAL_FOLDER" --strip-components=1

# Set the MONGO_HOME variable
export MONGO_HOME="$LOCAL_FOLDER"

# Display a message indicating successful completion
echo "MongoDB has been downloaded, extracted, and \$MONGO_HOME is set to $MONGO_HOME"


**Write a list of Linux commands to do the following:
Create a folder iit2022a. Change permissions of that folder to: owner (read write
execute), group (read write), others (read only). Write a Linux command to create a
file named final.txt. This file contains the text: “Final test is easy”. Change
permissions of that file to: owner (read write), group (read), others (none)**

* Create a folder named 'iit2022a'
mkdir iit2022a

* Change permissions of the folder to: owner (read write execute), group (read write), others (read only)
chmod 751 iit2022a

* Navigate to the created folder
cd iit2022a

* Write the text "Final test is easy" to a file named 'final.txt'
echo "Final test is easy" > final.txt

* Change permissions of the file to: owner (read write), group (read), others (none)
chmod 640 final.txt


**Write a bash script to print Hello World 1000 times.**
#!/bin/bash

* Loop to print "Hello World" 1000 times
for ((i=1; i<=1000; i++)); do
    echo "Hello World"
done
chmod +x hello_world_script.sh
./hello_world_script.sh

**How is Virtual Reality different from Augmented Reality? Discuss areas
where RMIT Vietnam can apply Virtual Reality and Augmented Reality into teaching
IT.**

Virtual Reality (VR) and Augmented Reality (AR) are both immersive technologies that alter our perception of the physical world, but they differ in their approaches and applications.

1. Definition:

- Virtual Reality (VR): VR creates a completely immersive, computer-generated environment that users can interact with. It replaces the real world with a simulated one, typically experienced through a headset.
- Augmented Reality (AR): AR overlays digital information onto the real-world environment. Users can see both the physical world and computer-generated content simultaneously, usually through devices like smartphones or AR glasses.
2. User Experience:

- VR: Offers a fully immersive experience, isolating users from the real world and transporting them to a virtual environment.
- AR: Enhances the real-world experience by adding digital elements. Users can still see and interact with the physical world while engaging with virtual content.
3. Devices:

- VR: Requires specialized hardware like VR headsets (Oculus Rift, HTC Vive, etc.) that completely occlude the user's vision.
- AR: Can be experienced on various devices, including smartphones, tablets, and AR glasses like Microsoft HoloLens or Google Glass.
4. Applications in Teaching IT at RMIT Vietnam:

- Virtual Labs (VR): Create virtual environments for students to conduct experiments, simulations, or practice programming in a safe and controlled setting.
AR Coding Assistance: Use AR overlays to provide real-time coding guidance and information, aiding students in learning programming languages and debugging.
- Virtual Campus Tours (VR/AR): Offer prospective students virtual or augmented tours of the campus, facilities, and IT labs to provide a more engaging and immersive experience.
- Collaborative VR Projects: Facilitate collaborative coding or IT projects in a VR space where students can work together, share ideas, and visualize complex concepts in three dimensions.
- AR Technical Documentation: Overlay technical information, schematics, or instructions onto physical IT equipment during hands-on lab sessions, enhancing the learning experience.
- VR Cybersecurity Simulations: Simulate real-world cybersecurity scenarios in VR environments, allowing students to practice and develop skills in a controlled and secure setting.
- AR for Visualizing Data Structures: Use AR to visualize complex data structures, algorithms, or IT architectures, making abstract concepts more tangible for students.
- VR IT Networking Simulations: Simulate networking scenarios in a virtual environment, allowing students to troubleshoot, configure, and understand networking concepts in a practical manner.


**In cyber security, what is social engineering attack? Give 3 examples.
Why are humans vulnerable to that type of attack?
0 words </>
5 ptsQuestion 3
3. (5 marks) How is Virtual Reality different from Augmented Reality? Discuss areas
where RMIT Vietnam can apply Virtual Reality and Augmented Reality into teaching
IT.**

Definition: Social engineering is a technique used by attackers to manipulate individuals into divulging confidential information or performing actions that compromise security.

Examples:

Phishing: Attackers send deceptive emails or messages, posing as a trustworthy entity, to trick individuals into revealing sensitive information such as passwords or financial details.

Pretexting: In this scenario, the attacker creates a fabricated scenario or pretext to extract information. For example, they might pose as a co-worker or support personnel to gain access to confidential data.

Baiting: Attackers offer something enticing, like a free software download or a tempting link, to lure individuals into clicking on malicious content that can lead to the compromise of their system.

Reasons for Human Vulnerability:

Trust and Social Compliance: Humans are naturally inclined to trust others and comply with social norms. Social engineers exploit this by impersonating trustworthy entities, making it easier to manipulate individuals.

Lack of Awareness: Many people are unaware of the various social engineering tactics and may not recognize warning signs or suspicious behavior.

Emotional Manipulation: Social engineering often involves emotional manipulation, preying on fear, urgency, or curiosity. When emotions come into play, individuals may act impulsively without critically evaluating the situation.

Complexity of Technology: As technology advances, the complexity of systems and interfaces can overwhelm users. This complexity may lead individuals to rely on seemingly helpful communication, making them susceptible to social engineering attacks.

Limited Security Training: Insufficient cybersecurity education and awareness training can leave individuals ill-equipped to identify and respond to social engineering attempts.


**In Cloud computing, what is Infrastructure as Service? Explain what is
the Economy of Scale in Cloud computing. Give 3 reasons why RMIT should migrate
their infrastructure to cloud?**


Infrastructure as a Service (IaaS) is one of the three main categories of cloud computing services, alongside Platform as a Service (PaaS) and Software as a Service (SaaS). In IaaS, the cloud provider offers virtualized computing resources over the internet. It allows users to rent virtualized hardware resources, such as servers, storage, and networking, on a pay-as-you-go basis. This eliminates the need for organizations to invest in and maintain physical hardware, providing flexibility and scalability.

* Economy of Scale in Cloud Computing:

The economy of scale in cloud computing refers to the cost advantages gained by cloud service providers due to the large scale and efficiency of their operations. This results in lower per-unit costs as the provider can spread its fixed costs over a larger number of customers and optimize resource utilization. The benefits of the economy of scale include:

- Cost Efficiency: Cloud providers can achieve cost efficiencies by aggregating demand and optimizing their infrastructure utilization. This enables them to offer services at a lower cost than what individual organizations would incur if they managed their own infrastructure.

- Flexibility and Scalability: Cloud providers can efficiently scale their infrastructure up or down based on demand. This flexibility allows organizations to pay only for the resources they use, avoiding the costs associated with overprovisioning or underutilization of resources.

- Access to Advanced Technologies: Cloud providers invest heavily in the latest technologies and hardware to stay competitive. Organizations leveraging cloud services can benefit from access to cutting-edge technologies without the need for substantial upfront investments.

* Reasons for RMIT to Migrate Infrastructure to the Cloud:

- Cost Savings: Migrating to the cloud can lead to significant cost savings for RMIT by eliminating the need for upfront investments in hardware, reducing maintenance costs, and optimizing resource utilization through pay-as-you-go pricing models.

- Scalability and Flexibility: Cloud platforms provide the flexibility to scale IT resources up or down based on demand. This scalability is particularly beneficial for educational institutions like RMIT, where resource requirements can vary during different academic periods.

- Focus on Core Competencies: By offloading infrastructure management to a cloud provider, RMIT can redirect its resources and expertise toward core educational and research activities, allowing the institution to focus on its primary mission without the distraction of managing complex IT infrastructure.

- Enhanced Security and Compliance: Reputable cloud providers invest heavily in security measures and compliance certifications. Migrating to the cloud can enhance the security posture of RMIT's IT infrastructure, ensuring data protection and regulatory compliance.

- Collaboration and Accessibility: Cloud-based solutions facilitate collaboration among students and faculty, providing easy access to resources and applications from any location with an internet connection. This enhances the overall learning experience and supports a more connected and collaborative academic environment.

