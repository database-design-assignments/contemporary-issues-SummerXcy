# IBM Security Launches Fully Homomorphic Encryption Services

##### Summer Xia 02.03.2021 cx534@nyu.edu

In this document, I will discuss the IBM Security Homomorphic Encryption Services, the concept of fully homomorphic encryption, its advantages and limitations through two articles. 

## Article 1 
In IBM's News Room ["IBM Helps Prepare Clients for Next Generation Encryption Technology"] (https://newsroom.ibm.com/2020-12-17-IBM-Helps-Prepare-Clients-for-Next-Generation-Encryption-Technology), as private data and information are shared more widely than ever before, we encrypt our data to keep it safe during storage and transfer. However, the data must be decrypted to be processed and thus created windows for data to be exposed. IBM is combating this problem using Fully Homomorphic Encryption (FHE), which enables computer to process sensitive data (eg. healthcare records and personal banking data) while it is still encrypted. 

FHE allows direct mathematical operations on encrypted data. For example, 5 + 10 can be encrypted as X + YZ. The result for X + YZ is PGD, and PGD can be decrpted as 15. 5 + 10 = 15 is correct. X + YZ = PGD is ciphertext calculation, and the operations on ciphertext are mirrored in plaintext after decryption. If we ask a third party to add or multiply values and return the result, we can then decrypt that result and get the correct answer. The third party doesn't have the key, thus never know the input or output. 

After solving the gap bewteen research and application, FHE will be a game changer for security in the hybrid cloud era, providing new business opportunities. Companies can acquire FHE tools, technical support, and a scalable hosting environemtn on IBM cloud to apply FHE in their unique industries. They can create FHE-enabled applications to leverage sensitive data while not worrying about confidentiality and privacy issues. 



## Article 2 
On ARS Technica, Jim Salter wrote an article ["IBM completes successful field trials on Fully Homomorphic Encryption"] (https://arstechnica.com/gadgets/2020/07/ibm-completes-successful-field-trials-on-fully-homomorphic-encryption/). This article goes beyond the praising and promoting of FHE in IBM's news, but also discussed limitations. 

The author mentioned how AMD's Secure Encrypted Virtualization can also solve the sysadmin problem where a system operator with root privileges can access to whatever data that is currently being operated on. With SEV, the operator who has root privilege could not scan or alter the contents of RAM in use "by a virtual machine running on that system". 

Fully Homomorphic Encryption offers other functions that Secure Encrypted Virtualization does not. However, there are also costs associated with FHE. The author gave an example on the machine-learning prediction task. FHE machine learning models need 40 to 50 times of additional computation power and 10 to 20 times of memory resources compared to what's needed for the same work on non-FHE encrypted models. 

Additionally, FHE has addition and multiplication, and all other mathmatical and logical operations are built based on the previous two. When performing operations on floating-point values, FHE decreases its accuracy for each operation, a small amount for addition and a larger amount for multiplication. With approximation approaches for many other mathematical statistics methods, it may be accompanied by the loss of accuracy and large calculation error.

But in all, FHE still has a very broad development space and application scenarios.



