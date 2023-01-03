# Dom Manipulation Assignment

# 1. Webiste Name: [Dev To](https://dev.to/)

### Topics

    - Query Selctory, Inner HTML

### Sample Image

![Sample One](./Images/Pic1.png)


### Tasks

        Target the Top description div and change the DEV Community to <Your_Name> and description to your passion

### Output

![Output](./Images/Pic2.png)

### Code
```
const sidebar = document.querySelector(".side-bar .crayons-card");

const tittle = sidebar.querySelector(".crayons-subtitle-2").innerHTML = "Hirenkumar"

const passion_desc = sidebar.querySelector("p");

passion_desc.innerHTML = "I create awsome web applications with the help of JavaScript language.
```
### Result
![Sample One](./Images/Ans1.PNG)

# 2. Website Name: [Apple](https://support.apple.com/en-in)

### Task

![Store](./Images/Picture_3.png)

### Fetch all the product name and store in an array

### Output

['iPhone', 'Mac', 'iPad', 'Watch', 'AirPods', 'Music', 'TV']

### Code
```
const devices = document.querySelector(".as-imagegrid .row");

const deviceChild = devices.children;

const Array = [];

for (const i of deviceChild) {
    const deviceName = i.getElementsByTagName("a")[0].getAttribute("data-analytics-link-component_name");
    Array.push(deviceName);
}
console.log(Array);

```
### Result
![Sample One](./Images/Ans2.PNG)


# # 3. Webiste Name: [Youtube Support](https://support.google.com/youtube/)

### Topics

    - Get Element By Id, Create Element, Create Text Node, Append Child

### Sample Image

![Sample One](./Images/Pic4.png)

### Tasks

     Add another FAQ 'My New FAQ' to the list

### Output
![Output](./Images/Pic5.png)

### Code
```
const accordian = document.querySelector(".accordion-homepage");

const mynewFaQ = document.createElement("section")
mynewFaQ.setAttribute("class", "parent")

const faq = document.createElement("h3")
faq.innerText = "My New FAQ"
faq.setAttribute("role", "button")
faq.setAttribute("aria-label", "My New FAQ")

mynewFaQ.appendChild(faq)

accordian.appendChild(mynewFaQ);
```
### Result
![Sample One](./Images/Ans3.PNG)



# 4. Webiste Name: [OnePlus](https://www.oneplus.in/support)

### Topics

     Query Selector, InnerText

### Sample Image

![Sample One](./Images/Pic6.png)

### Tasks

      Change the contact number

### Output

![Output](./Images/Pic7.png)

### Code
```
const telephoneEl = document.querySelector(".one-tel-number")

telephoneEl.innerText = "+91 6366256689";
telephoneEl.setAttribute("href", "tel:+91 1234567890")
```
### Result
![Sample One](./Images/Ans4.PNG)



# 5. Webiste Name: [Samsung](https://www.samsung.com/in/offer/online/samsung-fest/)

### Topics

       getElementById, createElement, InnerText, append, setAttribute

### Sample Image

![Sample One](./Images/Pic8.png)

### Tasks

     Target the main div of card and change the Button text to Check out

### Output

![Output](./Images/Pic9.png)

### Code
```
const checkout = document.querySelectorAll(".feature-column-carousel__button .cta")

for(let checkout of checkout) {
    checkout.innerText = "Check out"
}
```

### Result
![Sample One](./Images/Ans5.PNG)

# 6. Webiste Name: [Adidas](https://www.adidas.co.in/)

### Topics

    -   Query Selector, Event listeners, Changing Styles

### Sample Image

![Sample One](./Images/Pic10.png)

### Tasks

     Target the search box and on hover change thebackground color to red.

### Output

![Output](./Images/Pic11.png)

### code

```
const searchElement = document.querySelector(".searchinput___19uW0")

searchElement.addEventListener('mouseover', function (){
    searchElement.style.backgroundColor = "red";
});

```
### Result
![Sample One](./Images/Ans6.PNG)

# 7. Webiste Name: [MDN Web Docs](https://developer.mozilla.org/en-US/)

### Topics

       Form, Value, Submit

### Sample Image

![Sample One](./Images/Pic12.png)

### Tasks

     To Search a topic in the MDN Search bar.
     First add a text to search in the search bar and then hit the submit search button to search the docs using DOM

### Output

![Output](./Images/Pic13.png)

### code

```
const search = "CSS Positions";


const searchElement = document.getElementById("hp-search-input");
searchElement.value = search;

const formElement = document.querySelector("#hp-search-form")

formElement.submit();

```
### Result
![Sample One](./Images/Ans7.PNG)

# 8. Webiste Name: [Google](https://www.google.com/)

### Topics

       Remove Elements

### Sample Image

![Sample One](./Images/Pic14.png)

### Tasks

     Remove alternate languages from the home page languages listed

### Output

![Output](./Images/Pic15.png)

### code
```
const languages = document.getElementById("SIvCob");

const languagesList = document.querySelectorAll("#SIvCob a");

languagesList.forEach((i, j)=>{
    let index = j + 1;

    // remove odd element
    if(index % 2 !== 0) {
        languages.removeChild(i);
    }
})

```
### Result
![Sample One](./Images/Ans8.PNG)

# 9. Webiste Name: [Code Wars](https://www.codewars.com/)

### Topics

       Change Font Family, Color of Text.

### Sample Image

![Sample One](./Images/Pic16.png)

### Tasks

    Change the font family of the text to monospace and text color to the logo’s background color.

### Output

![Output](./Images/Pic17.png)

### code
```
const headingElement = document.querySelector("h1.display-heading-1");

headingElement.style.fontFamily = "monospace";
headingElement.style.color = "red";
```
### Result
![Sample One](./Images/Ans9.PNG)

# 10. Webiste Name: [Freecodecamp](https://www.freecodecamp.org/)

### Topics

       querySelector, mouseover, click eventListener,  callback function, style,

### Sample Image

![Sample One](./Images/Pic18.png)

### Tasks

    Target the button and change background colour on mouseover

### Output

![Output](./Images/Pic19.png)

### code
```
const button = document.querySelector(".signup-btn.btn-cta-big");

const btnText = button.querySelector(".signup-btn.btn-cta-big .login-btn-text")

button.addEventListener("mouseover", function(){
   btnText.style.backgroundColor = "red";
});
```
### Result
![Sample One](./Images/Ans10.PNG)

# 11. Webiste Name: [realme](https://www.realme.com/in/)

### Topics

       querySelector,style,background-image

### Sample Image

![Sample One](./Images/Pic20.png)

### Tasks

    change the realme logo to ineuron logo

### Output

![Output](./Images/Pic21.png)

### code

```
const iNeuronLogoPath = "https://ineuron.ai/Images/ineuron-logo.png";

const logo = document.querySelector("a.logo.gtag .icon-logo")

logo.style.backgroundImage = `url(${iNeuronLogoPath})`;

```
### Result
![Sample One](./Images/Ans11.PNG)

# 12. Webiste Name: [Github](https://github.com/)

### Topics

       querySelector,style,background-Color

### Sample Image

![Sample One](./Images/Pic22.png)

### Tasks

     change the background colour of the button to blue.

### Output

![Output](./Images/Pic23.png)

### code

```
const btn = document.querySelector(".js-repos-container a");

btn.style.backgroundColor = "blue";
```
### Result
![Sample One](./Images/Ans12.PNG)

# 13. Webiste Name: [Hackerrank](https://www.hackerrank.com/)

### Topics

       querySelector,innerHtml

### Sample Image

![Sample One](./Images/Pic24.png)

### Tasks

Target the top description and change “Matching developers with great companies” to ‘JSBOOTCAMP“.

### Output

![Output](./Images/Pic25.png)

### code

```
document.querySelector(".fl-heading-text").innerHTML = "JSBOOTCAMP"
```
### Result
![Sample One](./Images/Ans13.PNG)



# 14. Webiste Name: [Asus](https://www.asus.com/in/)

### Topics

      querySelector,style,font-size

### Sample Image

![Sample One](./Images/Pic26.png)

### Tasks

       change the fontsize of “Hot Deals” to 80px

### Output

![Output](./Images/Pic27.png)

### code

```
document.querySelector(".HotDealsAll__Heading__2fIbe").style.fontSize = "80px";
```

### Result
![Sample One](./Images/Ans14.PNG)

# 15. Webiste Name: [Dell](https://www.dell.com/en-in/shop/deals/laptop-deals?gacd=10415953-9016-5761040-285981356-0&dgc=ST&gclid=Cj0KCQjwguGYBhDRARIsAHgRm4-XUDMhhVNyHXb3s1gY4ZBzORr_d9Se-buhJwy7asyUe7YdqEA11eEaAt6UEALw_wcB&gclsrc=aw.ds&nclid=BxjBlpBQsX6pjSHh-L8YYSU77EpfXRkG1AGMB5Wbeu386ykspfrPDnfx_DdFau20)

### Topics

      querySelector,style.textAlign

### Sample Image

![Sample One](./Images/Pic28.png)

### Tasks

       Convert the text “G15 Gaming Laptop” from left to right

### Output

![Output](./Images/Pic29.png)

### code

```
const laptop = document.querySelector("#d560824win9b");

const title = laptop.querySelector(".ps-top .ps-title")

title.style.textAlign = "right";
```
### Result
![Sample One](./Images/Ans15.PNG)



# 16. Webiste Name: [Vercel](https://vercel.com/)

### Topics

     querySelector,innerHTMl

### Sample Image

![Sample One](./Images/Pic30.png)

### Tasks

      change the heading “Start with the developer” to “Start with Scratch”

### Output

![Output](./Images/Pic31.png)

### code

```
document.querySelector(".section-title_title__VEDfK").innerHTML = "Start with Scratch";
```
### Result
![Sample One](./Images/Ans16.PNG)

# 17. Webiste Name: [Sony](https://www.sony.co.in/)

### Topics

    querySelector,innerHTMl

### Sample Image

![Sample One](./Images/Pic33.png)

### Tasks

     change the button text To current Date.

### Output

![Output](./Images/Pic32.png)

### code

```
document.querySelector(".btn.buy.buy-button").innerHTML = new Date().toString();
```
### Result
![Sample One](./Images/Ans17.PNG)

# 18. Webiste Name: [Philips](https://www.philips.co.in/)

### Topics

     querySelector,style,backgroundcolor

### Sample Image

![Sample One](./Images/Pic34.png)

### Tasks

    change the background colour blue to orange

### Output

![Output](./Images/Pic35.png)

### code

```
document.querySelector(".p-f03-footer-container").style.background = "orange";
```
### Result
![Sample One](./Images/Ans18.PNG)


# 19. Webiste Name: [Canon](https://in.canon/)

### Topics

          querySelector,src

### Sample Image

![Sample One](./Images/Pic36.png)

### Tasks

    extract the canon logo

### Output

![Output](./Images/Pic37.png)

### code

```
document.querySelector(".logo").getAttribute("src");
```
### Result
![Sample One](./Images/Ans19.PNG)

# 20. Webiste Name: [Oppo](https://www.oppo.com/in/)

### Topics

          querySelector,style,color

### Sample Image

![Sample One](./Images/Pic38.png)

### Tasks

      Change the description colour black to orange

### Output

![Output](./Images/Pic39.png)

### code

```
document.querySelector(".wide h3.desc").style.color = "orange";

```
### Result
![Sample One](./Images/Ans20.PNG)

