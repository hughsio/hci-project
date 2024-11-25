________________________________________________________________________________________________________________________

##### Hugh Smith and Monique Boyd
##### Human Computer Interaction
##### Assignment 2

________________________________________________________________________________________________________________________

#### Evaluation of UDC.EDU Using Design Guidelines and Principles


### Introduction
The <a href="https://www.udc.edu" target="_blank">University of the District of Columbia</a> Website came online almost 30 years ago, and I'm going to assume that for most of that time, UDC has had some presence on the web via a website. Today, we will investigate the website's current version and highlight three good and lousy design features. We will highlight all the guidelines they violate or adhere to using the guidelines, principles, and theories outlined in Chapter 2.

### Design Flaw - Inconsistent Navigational Bar
![Inconsistent Design Example](images/inconsistent-navbar.gif)

#### Guidelines Violated
According to [Schneiderman’s Eight Golden Rule](https://www.cs.umd.edu/users/ben/goldenrules.html), “…identical terminology should be used in prompts, menus, and help screens; and consistent color, layout, capitalization, fonts, and so on, should be employed throughout.” The UDC website violates the this rule as well as the National Cancer Institute Digital Standards. We observed several instances of inconsistent menu bars on the UDC website that contravene these principle. In the highlighted image above, it is evident that the menu bar changes when navigating between pages.

The military page on the UDC website [www.udc.edu/military](www.udc.edu/military) offers crucial information to veterans and active military personnel. However, upon accessing the Veteran Service Organization page, we noticed discrepancies in the menu bar text size and color scheme, which differ from other pages. This inconsistency makes it challenging for users to navigate the site reliably.

Such inconsistencies can particularly confuse novice users, who may need to re-acquaint themselves with the interface on each page. This results in increased cognitive load diminished usability, and potential user frustration due to unpredictable navigation.

#### Supporting Principles and Theories
- [Shneiderman’s Rule](https://www.cs.umd.edu/users/ben/goldenrules.html): Striving for consistency ensures that users do not need to adjust their mental model for similar tasks or actions across a system.
- [NCI Digital Standards](https://www.cancer.gov/digital-standards): Consistent navigation patterns reduce cognitive load and ensure accessibility for all users.

#### Recommendations
- Standardize the Menu Bar: Use the same layout, color scheme, and terminology for the menu bar across all pages.
- Follow a Consistent Menu Order: Ensure menu items appear in the same sequence throughout the site.
- Test with Users: Conduct usability testing to confirm that the new menu design is intuitive and accessible for all user groups.


### Design Flaw - Blurred Image
![Blurred Image on Campus Master Plan Website](images/blurred-image.png)

### Guidelines Violated
The UDC website contains numerous images essential for conveying the message of each functional unit of the University. To effectively communicate these messages, the images must be high quality and visually pleasing. However, [UDC’s Campus Master Plan Page](https://www.udc.edu/facilities/campus-master-plan/) does not adhere to several design guidelines. These include the [National Cancer Institute’s Visual Standards](https://www.cancer.gov/digital-standards), which mandate that visual elements be professional and aesthetically pleasing, ensuring clarity and accessibility.
Additionally, the page violates [Web Content Accessibility Guidelines (WCAG) 1.4.5](https://www.w3.org/WAI/WCAG21/quickref/#images-of-text) (Images of Text): If an image contains text that becomes illegible due to blurriness, it directly contravenes accessibility standards. Lastly, it breaches [Shneiderman’s Rule 3](https://www.cs.umd.edu/users/ben/goldenrules.html) (Offer Informative Feedback): "Blurred images fail to convey clear, accurate information, diminishing the website’s usability." They images detract from a website's overall quality and professionalism, leading to multiple adverse effects. They undermine the user's trust and confidence in the website. When images are clear, users might perceive the website as poorly maintained or untrustworthy, which can drive them away.

#### Supporting Principles and Theories

- [National Cancer Institute’s Visual Standards](https://www.cancer.gov/digital-standards), which mandate that visual elements be professional and aesthetically pleasing, ensuring clarity and accessibility.
- [Web Content Accessibility Guidelines (WCAG) 1.4.5](https://www.w3.org/WAI/WCAG21/quickref/#images-of-text) (Images of Text): If an image contains text that becomes illegible due to blurriness, it directly contravenes accessibility standards.
- [Shneiderman’s Rule 3](https://www.cs.umd.edu/users/ben/goldenrules.html) (Offer Informative Feedback): Blurred images fail to convey clear, accurate information, diminishing the website’s usability.


#### Recommendations
- Replace Blurred Images: Ensure that high-resolution versions of images are uploaded and optimized for web use. Utilize formats such as PNG or JPEG with appropriate compression to maintain clarity.
- Use Scalable Formats: Consider employing vector graphics (SVG) for diagrams, charts, or logos to guarantee sharpness across various devices and resolutions.
- Test on Different Screens: Verify image quality across multiple devices, including desktops, tablets, and smartphones, to ensure consistency.


### Design Flaw - Missing Form Labels
![Missing Form Labels on Center for the Advancement of Learning Page](images/missing-form-label-2.gif)

### Guidelines Violated
The University’s website contains an extensive collection of crucial forms for business operations and student services. These forms ensure standardized data entry, essential for proper data management. The design of these forms plays a significant role in accessibility, as correctly formatted structures are necessary for screen readers and autofill suggestions to function effectively. The [Center For The Advancement of Learning’s Blackboard Course Restoration Form](https://www.udc.edu/cal/request-to-restore-blackboard-course/) violates several design guidelines rules, including the [Web Content Accessibility Guidelines (WCAG) 3.3.2](https://www.w3.org/WAI/WCAG21/quickref/#labels-or-instructions), which "requires that labels or instructions are provided when content requires user input." The intent is to ensure that users, especially those with disabilities, can understand what input is expected. In this case, it is important to ensure that screen readers can interpret the form well. In the Screenshot, we tested a screen reader’s ability to assess these form fields, and it could not read those fields due to missing labels. In addition to violating the WCAG guideline, this form violates the [United States Rehabilitation Act of 1973, Section 508](https://www.section508.gov/), and the [National Cancer Institute’s Digital Standards: Form Labels](https://www.cancer.gov/digital-standards/web-standards/forms). 


#### Supporting Principles and Theories

- [Web Content Accessibility Guidelines (WCAG) 3.3.2](https://www.w3.org/WAI/WCAG21/quickref/#labels-or-instructions)- WCAG 3.3.2, also known as Success Criterion 3.3.2: Labels or Instructions, is part of the Web Content Accessibility Guidelines (WCAG). This criterion requires that labels or instructions are provided when content requires user input. 
- [United States Rehabilitation Act of 1973, Section 508](https://www.section508.gov/) - Section 508 of the Rehabilitation Act of 1973, as amended, is a set of standards that requires federal agencies to make their Information and Communication Technology (ICT) accessible to employees and members of the public who have disabilities
- [National Cancer Institute’s Digital Standards: Form Labels](https://www.cancer.gov/digital-standards/web-standards/forms) - These standards include federal accessibility requirements and best practices in web design, ensuring that form labels are clear and accessible

#### Recommendations
Correct the follow HTML code by providing a label to the form. 
Here is the existing code for the current form which does not have a ``label`` attribute.

```
<input size="40" maxlength="400" class="wpcf7-form-control wpcf7-text wpcf7-validates-as-required" 
       id="firs-name" aria-required="true" aria-invalid="false" value="" 
       type="text" name="first-name">
```

Here is the corrected code:

`````
<label for="firs-name">First Name:</label>
<input size="40" maxlength="400" class="wpcf7-form-control wpcf7-text wpcf7-validates-as-required" 
       id="firs-name" aria-required="true" aria-invalid="false" value="" 
       type="text" name="first-name">
`````

### Design Strength - Responsive Website
![Website Displayed on the iPhone 14 Pro Max](/images/iPhone-14-ProMax.png)

Several guidelines govern the display of websites. A responsive website that adapts to various devices is essential to ensure an optimal user experience across different platforms. The World Wide Web Consortium (W3C) has established the [Web Content Accessibility Guidelines (WCAG)](), specifically [WCAG 2.1](https://www.w3.org/TR/WCAG21/) - Guideline 1.4.10, which stipulates that content must be presented without requiring horizontal scrolling or loss of information when viewed at a width of 320 pixels. This requirement ensures usability on smaller devices, such as smartphones.
Furthermore, [UDC’s website](https://www.udc.edu) conforms to [Shneiderman’s Rule 7: Support Flexibility and Efficiency of Use](https://www.cs.umd.edu/~ben/goldenrules.html). Responsive design accommodates different devices and screen sizes, offering flexibility for users accessing the site on mobile devices, tablets, or desktops.
The [NCI Digital Standards: Mobile and Responsive Design](https://www.cancer.gov/digital-standards/web-standards/responsive-design) emphasize prioritizing a responsive layout to cater to all users, regardless of device. This approach ensures that content and navigation remain accessible on screens of varying sizes.

### Supporting Principles and Theories
- [Web Content Accessibility Guidelines (WCAG)WCAG 2.1 - Guideline 1.4.10.](https://www.w3.org/TR/WCAG21/)
- [Shneiderman’s Rule 7](https://www.cs.umd.edu/users/ben/goldenrules.html)
- [NCI Digital Standards: Mobile and Responsive Design](https://www.cancer.gov/digital-standards#mobile-website-and-application-standards)



### Design Strength - Accessible Navigation with Keyboard
![Keyboard Navigation on UDC.EDU](/images/keyboard-navigation.gif)

Many users rely exclusively on keyboards to navigate websites, including individuals with motor disabilities, visual impairments (using screen readers), or temporary physical limitations, such as a broken arm. The UDC website is designed to be fully navigable using only a keyboard. Our testing involved using the Tab and Shift-Tab keys, which can enhance navigation efficiency for advanced users who prefer keyboard shortcuts. Supporting keyboard navigation on a website signifies compliance with global and federal accessibility standards. The [Web Content Accessibility Guidelines (WCAG), specifically WCAG 2.1 - Guideline 2.1.1 (Keyboard Accessibility)](https://www.w3.org/WAI/WCAG21/Understanding/keyboard-accessible), stress that all website functionality is operable through a keyboard without a mouse. This also complies with the [United States Rehabilitation Act of 1973, Section 508](https://www.section508.gov/) standards mandates that electronic content, including menus and links, is accessible to users who cannot operate a mouse. 

### Supporting Principles and Theories
- [Web Content Accessibility Guidelines (WCAG) WCAG 2.1 - Guideline 2.1.1 (Keyboard Accessibility)](https://www.w3.org/WAI/WCAG21/Understanding/keyboard-accessible)
- [United States Rehabilitation Act of 1973, Section 508](https://www.section508.gov/)


## Design Strength - Alternative Texts
![Alternative Text on Dr. April Massey's Bio page](/images/alt-text.png)

Screen readers help many users with visual impairments understand a website's content. For these users, alternative text (alt text) provides a textual description of images, allowing screen readers to announce the content or purpose of the image. Additionally, alt text is helpful when images fail to load, providing users context about the missing visual elements.

UDC’s website uses alt text for all non-decorative images, ensuring that users relying on assistive technologies can understand the meaning of visuals. Our testing included inspecting the website’s HTML for the presence of alt attributes and using a screen reader to verify that image descriptions were announced correctly. This approach improves accessibility for visually impaired users while benefiting all users when images cannot be displayed due to slow network connections.

Including alternative text on images aligns with global and federal accessibility standards. The [Web Content Accessibility Guidelines (WCAG), specifically WCAG 2.1 - Guideline 1.1.1 (Non-text Content)](https://www.w3.org/WAI/WCAG21/Understanding/non-text-content), emphasize providing text alternatives for all non-text content to make websites accessible. Furthermore, compliance with the [United States Rehabilitation Act of 1973](https://www.section508.gov/), Section 508 requires that all images convey equivalent information through alternative formats. It also complies with the [Americans with Disabilities Act (ADA) Title III Accessibility Requirements](https://www.ada.gov/law-and-regs/regulations/title-iii-regulations/) and the [National Cancer Institute Digital Standards – Accessibility guidelines](https://www.cancer.gov/digital-standards#accessibility-policy-section-508-compliance). 

Providing alt text supports universal design, ensuring accessibility for users with visual impairments, slow internet connections, and those using assistive technologies. It also helps websites comply with accessibility standards like WCAG, Section 508, and other global regulations.


### Supporting Principles and Theories
- [Web Content Accessibility Guidelines (WCAG), specifically WCAG 2.1 - Guideline 1.1.1 (Non-text Content)](https://www.w3.org/WAI/WCAG21/Understanding/non-text-content)
- [Americans with Disabilities Act (ADA) Title III Accessibility Requirements](https://www.ada.gov/law-and-regs/regulations/title-iii-regulations/)
- [National Cancer Institute Digital Standards – Accessibility guidelines](https://www.cancer.gov/digital-standards#accessibility-policy-section-508-compliance)