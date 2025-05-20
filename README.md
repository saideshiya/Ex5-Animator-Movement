# Ex5-Animator-Movement
## Aim:
To develop a animator movement for a player using unity.

## Algorithm:
## Step 1: 

Import necessary models.

## Step 2: 

 Right-click -> Create -> Animator Controller.

## Step 3: 

Open Animator window, define states (Idle, Run, Jump, etc.).

## Step 4: 

Use keyframes or Unity's Animation tools to animate transitions between states.

## Step 5: 

Drag Animator Controller to the GameObject in the Inspector.

## Program:

## Developed by: K. Sai Deshiya
## Reg no: 212224220084

## PlayerController:
```c#
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class PlayerController : MonoBehaviour
{
    public Animator animator;
    public float InputX;
    public float InputY;
    // Start is called before the first frame update
    void Start()
    {
        animator = this.gameObject.GetComponent < Animator>();
    }

    // Update is called once per frame
    void Update()
    {
        InputY = Input.GetAxis("Vertical");
        InputX = Input.GetAxis("Horizontal");
        animator.SetFloat("InputY", InputY);
        animator.SetFloat("InputX", InputX);
    }
}

```
## Output:
![Screenshot (51)](https://github.com/user-attachments/assets/7886a6c4-6558-4d6a-91f9-0246248655ca)
![Screenshot (52)](https://github.com/user-attachments/assets/226eee71-13ab-4739-98f0-674bbbf818ae)
![Screenshot (49)](https://github.com/user-attachments/assets/1618b8f8-5ab9-4504-a72a-17635e5abf81)


## Result:

An animator movement for a player using unity is developed successfully.


