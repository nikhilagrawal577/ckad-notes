# Stratergies-To-Crack-CKAD 
It includes a set of notes and practice test references to prepare for Certified Kubernetes Application Developer exam by Cloud Native Computing Foundation

**How to crack CKAD in 1st attempt**

Refer the below given link 
https://medium.com/@nikhilagrawal577/how-to-pass-ckad-exam-in-1st-attempt-tips-tricks-in-k8s-9e14477699ca



**Section Weightage Marks :**

 1. Core Concepts - 13% 
 2. Configuration - 18% 
 3. Multi-Container Pods - 10%
 4. Pod Design - 20% 
 5. State Persistence - 8% 
 6. Observability - 18% 
 7. Services and Networking - 13%

**Details :**

1. Core Concepts – 13%

-   Understand Kubernetes API primitives
-   Create and Configure Basic Pods

2. Configuration – 18%

-   Understand ConfigMaps
-   Understand SecurityContexts
-   Define an application’s resource requirements
-   Create & consume Secrets
-   Understand ServiceAccounts

3. Multi-Container Pods – 10%

-   Understand Multi-Container Pod design patterns (e .g. ambassador, adapter, sidecar)

4. Observability – 18%

-   Understand LivenessProbes and ReadinessProbes
-   Understand container logging
-   Understand how to monitor applications in Kubernetes
-   Understand debugging in Kubernetes

5. Pod Design – 20%

-   Understand how to use Labels, Selectors, and Annotations
-   Understand Deployments and how to perform rolling updates
-   Understand Deployments and how to perform rollbacks
-   Understand Jobs and CronJobs

6. Services & Networking – 13%

-   Understand Services
-   Demonstrate basic understanding of NetworkPolicies

7. State Persistence – 8%

-   Understand PersistentVolumeClaims for storage


### **Information About the Test:**

Once you schedule the test, you can’t reschedule or cancel it before 24hr of the scheduled test. You will get 1 free retake incase you didn’t qualify in first attempt.

_Here is the following details about the test._

-   2 hours : 19 questions
-   Remotely proctored in Chrome browser plus an extension
-   Government-issued Non-expired ID Card
-   Webcam and microphone
-   Completely practical, no theory. All on the command line
-   Questions are weighted with a percentage. Harder question, more points


#### **Use Imperative Commands**

I have noted down few imperative commands. It saves alot of time during the test. Practice these command as many times as you can. :D

1.  kubectl create service nodeport <myservicename>
2.  Kubectl expose Pod / Deployment — port=123 — name= Service_Name — namespace= Namespace_Name
3.  kubectl label / annotate / set / scale
4.  Kubectl run nginx — image=nginx — restart=Never — replicas=3
5.  K create secret generic abcd — from-literal=id=1
6.  K create congimap cm1 — from-literal=id=1

#### **Generating Yamls**

_Don’t try to write your own yamls at the exam._  
**_1. Pods , Deployments, Secrets, Configmaps, Jobs, Cron jobs_**  
These yamls can be generated using — dry-run , — export , -o yaml flags

    eg: k create deployment — image=nginx — dry-run -o yaml > dp.yaml

**_2. Persistent Volume, Persistent Volume Claim, Node Affinity, Node Selector, Service Account, Volumes_**  
These yamls can easily fetched from k8s.io documentations.

#### Editor

Be familiar with the editor you want to use. In my case , I have used Vi.  

**Things you should know better and fast in doing**
1.  Find and replace
2.  Going to exact line
3.  Deleting the word and line
4.  Checking the alignment
5.  Save & exit

### **Tips for the Exam**

1.  **Kubectl cheatsheet** : [https://kubernetes.io/docs/reference/kubectl/cheatsheet](https://kubernetes.io/docs/reference/kubectl/cheatsheet/)
2.  **Bookmarks :**  
    [https://github.com/nikhilagrawal577/ckad-notes/blob/master/CKAD_bookmarks.html](https://github.com/nikhilagrawal577/ckad-notes/blob/master/CKAD_bookmarks.html)  
    Just import in your browser and use it. I have added all relevant kubernetes.io document links.
3.  **Context :** Always pay attention to which context are you working ? It is correct or not. Make sure, you set the context before answering the actual question. Context will be given in the top of each question.
4.  If you are unsure of the spec or parameters of a yaml, always use `**kubectl explain <resource>.<key>**` Eg : `kubectl explain pod.spec`
5.  Time is extremely crucial. Try to read the question carefully and understand in a single go. **Don’t waste time in reading the question multiple times.**
6.  As weightage is already given for each question, if some less weightage question is taking more time to solve , you can skip and come back to that question later part of the test.
7.  Make sure, you are executing the commands in the **provided namespace**.
8.  **Be familiar with mouse or trackpad** as you need them to copy paste few names of the objects from the questions and to copy yaml from Kubernete.io page.
9.  Be an expert in terms of **Imperative commands** . It saves quite a lot of time.
10.  Don’t waste time in typing yaml codes. Generate Yamls

# Articles : 
1. https://matthewpalmer.net/kubernetes-app-developer/articles/ckad-practice-exam.html

2. https://www.avthart.com/posts/certified-kubernetes-exam-tips/
    
3. https://github.com/twajr/ckad-prep-notes#detailed-review

4. https://medium.com/@MrMcMuffins/ckad-exam-failure-748f978a325a

5. https://www.cloudreach.com/blog/study-guide-certified-kubernetes-application-developer-ckad-exam/

6. https://medium.com/chotot/tips-tricks-to-pass-certified-kubernetes-application-developer-ckad-exam-67c9e1b32e6e
	



# Courses :
1. https://training.linuxfoundation.org/certification/certified-kubernetes-application-developer-ckad/

2. https://www.katacoda.com/courses/kubernetes 

3. https://www.udemy.com/course/certified-kubernetes-application-developer/
	


# Practice Tests : 
1. https://github.com/dgkanatsios/CKAD-exercises [Highly recommended]

2. https://kodekloud.com/courses/kubernetes-certification-course/lectures/6743640

3. https://codeburst.io/kubernetes-ckad-weekly-challenges-overview-and-tips-7282b36a2681
	




## How to crack CKAD in 1st attempt

https://medium.com/@nikhilagrawal577/how-to-pass-ckad-exam-in-1st-attempt-tips-tricks-in-k8s-9e14477699ca
