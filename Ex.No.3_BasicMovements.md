# Ex.No: 3  Basic movements in Unity 
### DATE: 28-04-2024                                                                          
### REGISTER NUMBER : 212224240041
### Name : FRANKLIN.F
### AIM: 
 To learn the basic movements translation,scaling and rotation of game objects through code.
### Procedure:
1. Setup the Scene
2. Open Unity and create a 3D Scene.
3. Add three objects:Cube → Rename to Object1 (for movement),Sphere → Rename to Object2 (for rotation).Capsule → Rename to Object3 (for scaling).
4. Add the Script,Create a C# Script → Name it TransformOperations.cs.
5. Write the code for translation,scaling and rotation,save and close the script
6. Save the script
7. Select any empty GameObject (or create one: GameObject → Create Empty).
8. Attach the TransformOperations script to it.
9. In the Inspector, assign Object1 → Drag the Cube,Object2 → Drag the Sphere.Object3 → Drag the Capsule.
10. Run the Scene Press Play ▶️ in Unity
11. Stop the program.
### Program 
```
using UnityEngine;

public class FirstScript : MonoBehaviour
{
    public Transform object1;
    public Transform object2;
    public Transform object3;
    // Start is called once before the first execution of Update after the MonoBehaviour is created
    // start runs only once, when the script is first enabled. It is commonly used for initialization tasks that need to be performed before the game starts running.
    void Start()
    {
      print("Welcome to unity");  
    }

    // Update is called once per frame
    void Update()
    {
        if(Input.GetKeyUp(KeyCode.X))
        {
            object1.Translate(2f, 0, 0);
        }
        if(Input.GetKeyUp(KeyCode.Y))
            {
                object2.Rotate(20f, 0, 0);
            }
        if(Input.GetKeyUp(KeyCode.Z))
            {
                object3.localScale += new Vector3(2f, 2f, 2f);
            }

    }
}

```
### Output:
<img width="1903" height="1109" alt="image" src="https://github.com/user-attachments/assets/22081fa0-c7c1-4a04-b392-9136d5c47d35" />


### Result:
Thus the basic movement is learned through scripting


