# DEV277x-Object-Oriented-Programming-Java
Project Description

Company Structure

For this project you are going to practice using inheritance, interfaces and abstract classes to relate objects to one another. The following is a description of each class and its behavior. It is up to you to decide which classes should extend, implement or abstract which pieces to maximize your code sharing.

Create an object ecosystem that includes each of the following classes:

Employee

![employee](https://user-images.githubusercontent.com/95333101/148781448-4f88703f-aed7-4622-9272-169717fa2143.png)


TechnicalEmployee
![te](https://user-images.githubusercontent.com/95333101/148781471-99d0a6b0-4afe-45e7-b0fb-56b520ab079a.png)



BusinessEmployee
![be](https://user-images.githubusercontent.com/95333101/148781500-0b97990a-6727-4a77-b92f-2e50fd9570c1.png)


SoftwareEngineer
![se](https://user-images.githubusercontent.com/95333101/148781529-f970ad4b-1f78-4c6e-9d02-b3cc7eea28ad.png)


Accountant
![accountant](https://user-images.githubusercontent.com/95333101/148781574-9f4c30d0-b692-4047-9634-94699ffc337c.png)


TechnicalLead

![tl](https://user-images.githubusercontent.com/95333101/148781601-b330fd58-b3eb-4524-9ef0-846b084537d1.png)


BusinessLead

![bl](https://user-images.githubusercontent.com/95333101/148781622-7d75c680-f39f-4580-be1c-0cf2ee385bed.png)


Here is my testing code that you can use to see if things are set up properly:
public class CompanyStructure {
public static void main(String[] args) {
TechnicalLead CTO = new TechnicalLead("Satya Nadella");
SoftwareEngineer seA = new SoftwareEngineer("Kasey");
SoftwareEngineer seB = new SoftwareEngineer("Breana");
SoftwareEngineer seC = new SoftwareEngineer("Eric");
CTO.addReport(seA);
CTO.addReport(seB);
CTO.addReport(seC);
System.out.println(CTO.getTeamStatus());
TechnicalLead VPofENG = new TechnicalLead("Bill Gates");
SoftwareEngineer seD = new SoftwareEngineer("Winter");
SoftwareEngineer seE = new SoftwareEngineer("Libby");
SoftwareEngineer seF = new SoftwareEngineer("Gizan");
SoftwareEngineer seG = new SoftwareEngineer("Zaynah");
VPofENG.addReport(seD);
VPofENG.addReport(seE);
VPofENG.addReport(seF);
VPofENG.addReport(seG);
System.out.println(VPofENG.getTeamStatus());
BusinessLead CFO = new BusinessLead("Amy Hood");
Accountant actA = new Accountant("Niky");
Accountant actB = new Accountant("Andrew");
CFO.addReport(actA, CTO);
CFO.addReport(actB, VPofENG);
System.out.println(CFO.getTeamStatus());
}
}
