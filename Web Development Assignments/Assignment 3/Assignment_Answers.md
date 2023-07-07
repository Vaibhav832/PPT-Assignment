# Q1 What is media query in CSS, What is it's purpose?

Ans: Media queries allow you to apply CSS styles depending on a divece's general type (such as print vs screen) or other characteristics such as screen resolution or browser viewport width.

### It's purposes

Media queries can be used to check many things such as

- width and height of the viewport
- width and height of the device
- orientation (is the tab/ phone in landscape or portrait)
- resolution

<br/>

# Q2. How do you define a media query in CSS?

Ans: Media queruies are basically a way to write conditional css. That means CSS markup that the browser will only render if certain conditions are met. It is used in responsive design where its a way to tell the browser to change the display of website elements when above or below certain screen size

### syntax

```css
@media screen and (min-width: 680px);
```

<br/>

# Q3. Explain the concept of breakpoints in responsive web design and how they are used in media queries?

Ans: Breaking points are building blocks of responsive design. Its a value that determines a website's size and layout across different screen sizes.
Breakpoints creates a responsive website design when implemented with a CSS media query

# Q4. What is the purpose of using media queries for print media?

Ans: Media queries can also be used to create print styles using `@media print`

```css
@media print {
  #header,
  #footer,
  #nav {
    display: none !important;
  }
}
```

# Q5. What is the purpose of the `orientation` media feature?

Ans: The orientation CSS media feature can be used to test the orientation of the viewport.
The orientation feature is specified as a keyword value chosen from the list below

- potrait: that is the height is greater or equal to the width
- lanscape: the width is greater than the height

# Q6. The OneCard website clone- fully responsive

[source code](https://github.com/Vaibhav832/PPT-Assignment/tree/main/Web%20Development%20Assignments/Assignment%203/OneCardWebsiteClone)

<img width="960" alt="image" src="https://github.com/Vaibhav832/PPT-Assignment/assets/81919583/3649d2af-4151-46ba-b208-02de3a535e61">
<img width="960" alt="image" src="https://github.com/Vaibhav832/PPT-Assignment/assets/81919583/a1d8cca4-5c9b-492f-ae05-a7bf5489c1ae">

# Q7. The image gallery using grid layout- fully responsive

[source code](https://github.com/Vaibhav832/PPT-Assignment/tree/main/Web%20Development%20Assignments/Assignment%203/ImageGallery)

![1](https://github.com/Vaibhav832/PPT-Assignment/assets/81919583/1464a5f2-3cc5-4719-919e-f66fafac8bb6)
![2](https://github.com/Vaibhav832/PPT-Assignment/assets/81919583/be07de7f-beb0-4465-8eb9-22f1981f99ac)
![3](https://github.com/Zareel/PlacementAssignment_ZareelKalam/assets/110910838/01beb8de-42bf-408b-a46a-28a327c647d3)

# Q8 Dark mode and light mode- fully responsive

[source code](https://github.com/Vaibhav832/PPT-Assignment/tree/main/Web%20Development%20Assignments/Assignment%203/DarkModeAndLightMode)

![1](https://github.com/Zareel/PPT-Web-Development-Assignments/assets/110910838/06f13c60-fd45-43f0-95fc-9e8ce44ded25)
![2](https://github.com/Zareel/PPT-Web-Development-Assignments/assets/110910838/8358d8d7-286d-4a50-9392-4e22a807428a)

# Q9. Footer- fully responsive

[source code](https://github.com/Vaibhav832/PPT-Assignment/tree/main/Web%20Development%20Assignments/Assignment%203/ResponsiveFooter)
![1](https://github.com/Zareel/PPT-Web-Development-Assignments/assets/110910838/4314c531-ac3d-4ac2-8e32-aafd9114179c)
![2](https://github.com/Zareel/PPT-Web-Development-Assignments/assets/110910838/ba32d9bd-0ef9-46a7-b351-2b73beef3881)

# Q10 Student dashboard

[source code](https://github.com/Vaibhav832/PPT-Assignment/tree/main/Web%20Development%20Assignments/Assignment%203/StudentDashboard)

![1](https://github.com/Zareel/PPT-Web-Development-Assignments/assets/110910838/daefa369-a9e9-4801-bf02-c4868b7960f6)

<br>

![2](https://github.com/Zareel/PPT-Web-Development-Assignments/assets/110910838/5f59d6f9-0d6e-46bf-9971-817e40b1858f)
