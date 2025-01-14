
#### user journey
```mermaid
journey
    title Brocks working day
    section Go to work
      Make tea: 5: Me, Brock, 
      Go upstairs: 3: Coco
      Do work: 1: Me, Courtney
    section Go home
      Go downstairs: 5: Me
      Sit down: 5: Me
```

#### sequence diagram
```mermaid
sequenceDiagram
    title Conversation
    Alice->>John: Hello John, how are you?
    John-->>Alice: Great!
    Alice-)John: See you later!
```
**block diagram**  
```mermaid
block-beta
  columns 3
      
  a:3       
  
  block:group1:2   
    columns 2      
    h i            
    j k            
  end            
  
  g             
  
  block:group2:3   
    l m n               
  end  


  block:group3:3   
    x               
  end  
```


#### quad chart
```mermaid
quadrantChart
    title Reach vs Engagement
    x-axis Low Reach --> High Reach
    y-axis Low Engagement --> High Engagement
    quadrant-1 We should expand
    quadrant-2 Need to promote
    quadrant-3 Re-evaluate
    quadrant-4 May be improved
    Campaign A: [0.3, 0.6]
    Campaign B: [0.45, 0.23]
    Campaign C: [0.57, 0.69]
    Campaign D: [0.78, 0.34]
    Campaign E: [0.40, 0.34]
    Campaign F: [0.35, 0.78]
```


```mermaid
classDiagram
    note "From Duck till Zebra"
    Animal <|-- Duck
    note for Duck "can fly\ncan swim\ncan dive\ncan help in debugging"
    Animal <|-- Fish
    Animal <|-- Zebra
    Animal : +int age
    Animal : +String gender
    Animal: +isMammal()
    Animal: +mate()
    class Duck{
        +String beakColor
        +swim()
        +quack()
    }
    class Fish{
        -int sizeInFeet
        -canEat()
    }
    class Zebra{
        +bool is_wild
        +run()
    }
```

```mermaid
---
title: Example Git diagram
---
gitGraph
   commit
   commit
   branch develop
   checkout develop
   commit
   commit
   checkout main
   merge develop
   commit
   commit
```




## Examples

**cprs login journey**

PROMPT:  
create user journey diagram in mermaid for the documentation provided for login to a client

USER:  
copy/paste CPRS user guide section on logging in

OUTPUT (ChatGPT):  
Based on the documentation provided, here's a detailed user journey diagram in Mermaid for logging into CPRS using both two-factor authentication with a PIV card and the alternative method with access and verify codes.  



```mermaid
journey
    title CPRS Login Journey
    section Login with PIV Card
      User double-clicks CPRS icon: 5: User
      User selects appropriate account if prompted: 3: User
      User chooses certificate associated with PIV card: 4: User
      User enters PIN: 4: User
      System validates PIN and grants access: 3: System
      User is logged into CPRS: 5: User
    section If PIV Card Fails
      User selects Cancel: 4: User
      User opts to use access and verify codes: 4: User
    section Login with Access and Verify Codes
      User double-clicks CPRS icon: 5: User
      User selects appropriate account if prompted: 3: User
      User enters access code: 4: User
      User enters verify code: 4: User
      System validates access and verify codes: 3: System
      User is logged into CPRS: 5: User
```


**user journey**
```mermaid
journey
    title User Login Journey
    section Navigate to Login Page
      User navigates to the login page: 5: User
    section Enter Credentials
      User enters username: 4: User
      User enters password: 4: User
    section Submit Login Form
      User clicks the "Login" button: 5: User
    section Validate Credentials
      System validates credentials: 3: System
    section Grant Access
      System grants access: 4: System
      User is redirected to the dashboard: 5: User
```

**block diagram**  
https://mermaid.js.org/syntax/block.html#column-width-dynamics  


```mermaid
block-beta
  columns 3
  a:3
  block:group1:2
    columns 2
    h i j k
  end
  g
  block:group2:3
    %% columns auto (default)
    l m n o p q r
  end
```

**flowchart**  
```mermaid
flowchart TD;
    A[Start] --> B[Process 1];
    B --> C[Process 2];
    C --> D[End];
```

**graph**
```mermaid
graph TD;
    A[Outer Box] --> B[Inner Box 1];
    A --> C[Inner Box 2];

    B --> D[Sub Box 1];
    B --> E[Sub Box 2];

    D --> F[Sub Sub Box 1];
    D --> G[Sub Sub Box 2];

    C --> H[Sub Box 3];
    C --> I[Sub Box 4];

