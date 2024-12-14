# S-tasks

## Task II

### Blog

Creating Dynamic Watch Faces with [Watch Face Studio](https://developer.samsung.com/watch-face-studio/overview.html): A Step-by-Step Guide
Smartwatches are more than just functional gadgets; they are extensions of personal style and utility. For designers and developers, crafting custom watch faces offers an exciting opportunity to combine creativity with functionality. Samsung’s Watch Face Studio (**WFS**) provides an intuitive platform that enables anyone—whether you're a seasoned developer or a design enthusiast—to create interactive and stunning watch faces without writing a single line of code.

In this blog, we’ll explore the process of designing a dynamic analog watch face that incorporates essential features like battery level indicators and charging status. Using tag expressions, we’ll bring interactivity and intelligence to the watch face, ensuring it responds to user context, such as low battery warnings and charging status.

This **guide** will walk you through every step, from setting up WFS and designing components to previewing and publishing your creation. Whether you're a beginner or an experienced watch face designer, you'll learn how to use the tools and techniques to build a functional and visually appealing watch face.

---
---

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/739c75a5-7984-43df-9012-d181bab289fd" alt="Image 1" style="width:400px; height:400px; border-radius:10px;"><br>
      <b>Normal</b>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/54ac7bc3-85df-46f8-9dd7-fd612201abad" alt="Image 2" style="width:400px; height:400px; border-radius:10px;"><br>
      <b> AlwaysOn State </b>
    </td>
  
  </tr>
</table>


---
---
### Step 1: Installation and Setup

To **begin** the process of creating a custom watch face, the first step is to install Watch Face Studio (WFS), Samsung's official design tool for Wear OS devices. This tool is designed to make it easier for both beginners and experienced developers to create unique, interactive, and functional watch faces without needing any coding knowledge.
Once Watch Face Studio is installed, the next step is to set up the testing environment. For this, an Android device running Wear OS must be properly configured. This allows you to test the watch face design in real-time on an actual device, ensuring that the watch face functions as expected before finalizing the design. [Guide](https://developer.samsung.com/watch-face-studio/overview.html)

---

### Step 2: Creating a New Project

After setting up the environment, the next step was to **create a new project** in Watch Face Studio.

---

### Step 3: Adding Components – Index Selection

After setting up the project, the next step is enhancing the watch face design by adding key components. The first component to add is the **Index**.

In Watch Face Studio, an **Index** represents the markers or numerals on an analog watch face that indicate the hours. These elements are fundamental to any traditional watch design, making it easy for users to read the time at a glance.

How to Add an **Index**
- Open the **Add Component** menu and select **Index** from the list.
- For this design, the **index_simple** component is selected as it provides a clean and minimalistic appearance.
- Once the **Index** is added, you can customize its properties:
- Color: Adjust the color to match your design’s aesthetic or branding.
- Themes: Apply a theme to the **Index** to provide dynamic styling options, enabling users to personalize their watch face.

The index not only enhances the readability of the watch face but also contributes to its overall visual appeal, providing a blend of functionality and style.


<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/e77fce5b-271e-4fc7-80e2-b03fedb0d04b" alt="Image 1" style="width:200px; height:200px; border-radius:10px;"><br>
      <b>Add Component Section</b>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/6dd5029b-e922-41dc-bb99-1a2b594aa7b8" alt="Image 2" style="width:400px; height:150px; border-radius:10px;"><br>
      <b>Selecting index from add component</b>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/fa6c1d52-2a2d-4104-bedf-4034efd04e28" alt="Image 3" style="width:200px; height:200px; border-radius:10px;"><br>
      <b>Current Layer</b>
    </td>
  </tr>
</table>


---

### Step 4: Adding the Analog Clock Component

The next essential component to add is the **Analog Clock**. To do this, select **Analog Clock** from the **Add Component** menu and rename it to **Default Analog Clock**.

The Analog Dial serves as the core structure of any analog watch face, displaying time through rotating hands. In Watch Face Studio, this component can be fully customized, including adjusting colors, sizes, and designs, allowing for a personalized touch. For this design, the default Analog Dial is chosen for simplicity, as it offers a clean and functional layout that is ideal for users who prefer a straightforward analog watch face without complex customizations.

Although the default option is used, you still have the flexibility to modify its individual components, such as adjusting the color of the hour, minute, and second hands to align with your design theme. This ensures that even a default setup can be tailored to suit your unique style.


<img src="https://github.com/user-attachments/assets/d5a3fdaa-a330-48f3-affa-32a8a02790d0" alt="Screenshot 1" width="50%"/>  



---

### Step 5: Adding a Battery Circle Complication

**Complications** are customizable elements on a watch face that display dynamic information, such as battery status, heart rate, weather updates, or other relevant data. For this design, the focus is on the **battery status**, though complications like heart rate or step count can easily be added.

To add the **Battery Circle Complication**, click the **Add Component** button again and select **Circle Complication** from the available options. This component provides a circular gauge to visually represent the watch's current battery level. For clarity, rename the newly added **Circle Complication** to **Default Battery Component**.

Once the component is added, **configure** it to display the battery percentage. The UI of the component is fully customizable, offering flexibility in adjusting its color, size, and position on the watch face. Although the default configuration is used initially, you can easily modify it to better align with the overall design theme, ensuring a seamless and cohesive look.

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/e26252f6-7f4b-49e3-b5b1-1f66840c6801" alt="Image 1" style="width:400px; height:250px; border-radius:10px;"><br>
      <b>Current Layer</b>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/d5658db5-a5ac-46e7-b61d-9a6d06e1b3f9" alt="Image 2" style="width:200px; height:300px; border-radius:10px;"><br>
      <b>Complication settings of Default Battery Component </b>
    </td>
  
  </tr>
</table>

---

#### Understanding Tag Expressions in Watch Face Studio

[**Tag expressions**](https://developer.samsung.com/watch-face-studio/user-guide/tag-expression.html) are powerful tools in Watch Face Studio (WFS) that enable designers to add dynamic, real-time behavior to their watch faces without writing any code. These expressions allow for modifications to properties like color, opacity, size, and position, based on live data such as battery percentage, time, or heart rate.

The basic syntax for a **tag expression** is as follows:

**[CONDITION] ? [TRUE_VALUE] : [FALSE_VALUE]**

In this structure:
- [CONDITION] refers to a specific condition or variable, such as battery percentage or time of day.
- [TRUE_VALUE] is the value applied when the condition is met.
- [FALSE_VALUE] is the value applied when the condition is not met.

Tag expressions make watch faces more interactive and responsive to real-time data, offering a richer user experience by providing dynamic visual feedback.

For example, **by using a tag expression, the opacity of the battery circle can change based on the battery level. If the battery percentage is above 20%, the circle remains fully visible. However, if the battery percentage drops to 20% or below, the circle becomes completely transparent, visually signaling a low battery status. This is how you can implement such a dynamic feature.**

---

### Step 6: Adding Dynamic Visual Feedback

To provide dynamic visual feedback, **select Text, Icon, and Progress Bar components together in the Layer Layout. On the right side, you’ll find the Properties Panel for the selected items. In the Color section, we will modify the opacity of the battery circle using a tag expression for these three components.**

The tag expression used for this is:

**[BATT_PER] > 20 ? 0 : -100**

Here’s how this expression works:

[BATT_PER] refers to the battery percentage of the watch.
- 20 checks if the battery percentage is greater than 20%.
- 0 sets the opacity to 0, making the component fully visible when the battery level is above 20%.
- 100 sets the opacity to -100, making the component fully transparent when the battery level is at or below 20%.
  
This tag expression ensures that the battery circle dynamically adjusts its opacity based on the battery level, providing users with clear visual feedback on their device's battery status.


<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/98eb73f0-ad42-4e04-8c35-ac8cd58f85a4" alt="Image 1" style="width:200px; height:300px; border-radius:10px;"><br>
      <b>Selecting 3 components</b>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/dc3f6464-d1ae-436d-b86e-6adf435bb112" alt="Image 2" style="width:350px; height:300px; border-radius:10px;"><br>
      <b>Adding opacity tag for 3 items </b>
    </td>
  
  </tr>
</table>

---

### Step 7: Enhancing with a Low Battery Indicator

To provide a clearer visual cue for **low battery status**, the default Battery Component is **duplicated**. The duplicated component is renamed to **Low Battery Component** for better clarity and easier identification.

**In the Low Battery Component, the Text Icon Progress Bar is selected, offering a clear visual representation of the battery level in a progress bar style. After selecting the appropriate elements for the progress bar, the color is changed to red to indicate that the battery level is critically low.**

To further enhance the dynamic behavior, a **tag expression** is added to control the **opacity** of the component based on the **battery percentage**. The tag expression used is:
**[BATT_PER] > 20 ? 0 : -100**



<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/d410df9d-2212-420e-8286-18f599d9d3e1" alt="Image 1" style="width:400; height:250px; border-radius:10px;"><br>
      <b>Selecting 3 low battery components</b>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/c0a37216-cde5-4876-bc0a-6758c766bcc0" alt="Image 2" style="width:300px; height:200px; border-radius:10px;"><br>
      <b>Changing tag expression and color </b>
    </td>
  
  </tr>
</table>


This expression ensures that the **Low Battery Component remains fully visible when the battery level is above 20%, and becomes completely transparent when the battery level drops to 20% or below. This dynamic behavior provides immediate feedback to users regarding the battery status, enhancing the overall watch face experience.**

---

### Step 8: Adding a Charging Status Complication

To make the watch face even more informative, a **Charging Status Complication** is added. This complication visually indicates when the smartwatch is charging, offering users real-time feedback on the device's power status.

Steps to Add the Charging Icon:

- Navigate to the **Add Component** menu and select **Image** from the list of available components.
- This image will serve as the charging icon, indicating when the watch is charging.
- Select **any** image, to visually signify the charging status.
- Position the image on the watch face in a way that ensures visibility without interfering with other elements on the screen.

Configure the Image Properties:

**In the Properties Panel, go to the Color section.
Add the following tag expression in the color field to dynamically adjust the visibility of the charging icon:**

**[BATT_IS_CHARGE] == 1 ? 0 : -100**

This **expression** ensures that the charging icon becomes fully visible when the watch is charging (i.e., [BATT_IS_CHARGE] == 1), and remains hidden when the watch is not charging.
By following these steps, you integrate a charging status indicator into the watch face, further enhancing its functionality and providing users with a clear view of their device's charging status. Final layer will look like this: 
<img src="https://github.com/user-attachments/assets/28cb9dd3-c5bd-464f-8676-b7204df81327" alt="Screenshot 1" width="50%"/>  

---

### Step 9: Preview and Publish the Watch Face

Once all components and configurations are complete, the next step is to **preview** the watch face to ensure everything functions as intended.

Preview the Watch Face:
1. Run the Preview:

- Utilize the **built-in preview option** in Watch Face Studio (WFS) to simulate how the watch face will appear and behave on an actual device.
- While previewing, verify the following:
-- The analog hands and indexes display correctly.
-- The battery circle complication dynamically updates based on the current battery percentage.
-- The Low Battery Component turns red and becomes visible when the battery drops to 20% or below.
-- The charging icon only appears when the watch is charging.


2. Test on a Device:
- If a physical **Wear OS** smartwatch is available, transfer the watch face to the device using the test on device feature.
- Ensure that the watch face is responsive and visually aligned on the device's screen, making adjustments if necessary.

3. Publishing the Watch Face:
If the watch face meets all the desired requirements and is ready for public use, proceed with the following steps to publish it:
- Navigate to the Project menu and select Upload. This prepares the project for submission, making it available for public distribution.
  
By following these steps, you ensure that the watch face is thoroughly tested and ready for release, providing users with a polished, functional product.

To learn more check the [official documentation](https://developer.samsung.com/watch-face-studio/user-guide/create.html), or watch [this](https://www.youtube.com/watch?v=kOGvl3CaTgM).
