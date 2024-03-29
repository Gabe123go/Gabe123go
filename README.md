- 👋 Hi, I’m @Gabe123go
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Gabe123go/Gabe123go is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
Certainly! Here is a simple script in Unity using C# that creates a button you can press:

```csharp
using UnityEngine;
using UnityEngine.UI;

public class ButtonPress : MonoBehaviour
{
    void Start()
    {
        // Create a new button
        GameObject buttonGameObject = new GameObject("Button");

        // Add Button component to the button GameObject
        Button button = buttonGameObject.AddComponent<button>();
        button.onClick.AddListener(OnButtonClick);

        // Set the button's text
        Text buttonText = buttonGameObject.AddComponent<text>();
        buttonText.text = "Press Me";

        // Set the position of the button on the screen
        RectTransform rectTransform = buttonGameObject.GetComponent<recttransform>();
        rectTransform.SetParent(this.transform, false);
        rectTransform.localPosition = new Vector3(0, 0, 0);
    }

    void OnButtonClick()
    {
        Debug.Log("Button Pressed!");
    }
}
```

To use this script in Unity, follow these steps:
1. Create an empty GameObject in your scene.
2. Attach the above script to the empty GameObject.
3. Press play in the Unity Editor and you should see a button labeled "Press Me".
4. Click on the button and you will see the message "Button Pressed!" logged in the console.

Feel free to customize the button's appearance and functionality further as needed. Let me know if you have any questions or need further assistance!</recttransform></text></button>
