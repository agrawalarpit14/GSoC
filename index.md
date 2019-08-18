---
layout: report
url: agrawalarpit14
student: Arpit Agrawal
organisation: OWASP Foundation (Juice Shop Project)
organisation_link : https://www.owasp.org/index.php/OWASP_Juice_Shop_Project
project: Feature Pack 2019
project_link: https://summerofcode.withgoogle.com/projects/#5592124823699456
mentors: >
 [Björn Kimminich](https://github.com/bkimminich) & [Jannik Hollenbach](https://github.com/J12934) & [Shoeb Patel](https://github.com/CaptainFreak)
bio: >
 I am presently pursuing a degree in Computer Science and Engineering, at the Indian Institute of Technology, Dharwad. From the age of fifteen, I have been exploring the field of Computer Security and have developed a strong passion for it. I started in this field, by reading various research papers and blogs, auditing online courses and tutorials and implementing the learned tricks and tools. I even managed to find security vulnerabilities in my college network. An early motivator in my open-source journey was my first commit to the Metasploit Framework. As days progressed, I was introduced to OWASP and Juice Shop then became my major source of learning.
social:
 - GitHub:
   - username: agrawalarpit14
   - link: https://github.com/agrawalarpit14
 - GitLab:
   - username: agrawalarpit14
   - link: https://gitlab.com/agrawalarpit14
email: agrawal.arpit14@gmail.com
blog: http://hemangsk.github.io/stories.html
activity:
 - 0:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/980
   - details: > 
      Implementation of multiple user types
 - 1:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/982
   - details: >
      Implementation of stock inventory
 - 2:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1044
   - details: > 
      Implementation of Accounting user
 - 3:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1056
   - details: > 
      Implementation of limit on the purchase of specific items 
 - 4:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1108
   - details: Add address component 
 - 5:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1120
   - details: Implementation of Payment Method Component
 - 6:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1121
   - details: Add Order Summary Page
 - 7:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1123
   - details: Add quantity labels
 - 8:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1127
   - details: Quantity refactoring
 - 9:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1130
   - details: Add Order Confirmation Page
 - 10:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1151
   - details: Fix Build, Modify Data Type
 - 11:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1152
   - details: Payment component
 - 12:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1168
   - details: Implement Delivery methods
 - 13:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1170
   - details: Pre-store Addresses and Cards, Change card expiry year range
 - 14:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1171
   - details: Implement Order History
 - 15:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1174
   - details: Implement Digital Wallet View
 - 17:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1178
   - details: Implement Deluxe Membership Purchase View
 - 18:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1179
   - details: Make icons green according to the status of an order
 - 19:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1180
   - details: Implement Photo wall
 - 20:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1183
   - details: Make delivery box image customizable
 - 21:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1184
   - details: Merge payment routes
 - 22:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1186
   - details: Add memory to data export, add twitter button
 - 23:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1187
   - details: Add addresses to recycle component
 - 24:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1189
   - details: Deals & Offers for deluxe members
 - 25:
   - repo: juice-shop
   - link: https://github.com/bkimminich/juice-shop/pull/1191
   - details: Fix code errors
 - 26:
   - repo: pwning-juice-shop
   - link: https://github.com/bkimminich/pwning-juice-shop/pull/42
   - details: Update happy path

---

### Feature Pack 2019

#### Features
The project can be broken down in terms of the following features.

<ol>
  <li>
    <b>Stock Inventory</b>
    : Maintaining stocks of available products in the Juice Shop brings it very close to the realistic scenarios where people are unable to order the desired quantity of goods either due to unavailability or due to restriction on the quantity of an item.
  </li>
  <li>
   <b>Payment Gateway</b>
   : With this additional feature users will be able to pay for their products(no money actually involved; dummy/fake cards) and experience hacks built around the vulnerabilities in the e-payment process.
  </li>
  <li>
   <b>Juice Shop Wallet</b>
   : Many online vendors integrate their own digital wallet to smoothen the payment process. By integrating juice shop’s wallet we can expose users to a new range of attacks including identity theft, request tampering, and access token manipulation.
  </li>
  <li>
   <b>Delivery methods and Order history</b>
   : This feature can be added to involve scheduling of events in the juice shop (which can be home to various challenges) and this also brings it very close to the realistic scenario where people have multiple options to choose for the delivery service(depending on how early they need their products vs how much they are willing to pay).
  </li>
  <li>
   <b>Juice Shop Prime Membership</b>
   : A feature to provide privileged membership to the users of the juice shop giving them various benefits such as free one day delivery, no quantity limits on the purchase and special deals and offers in exchange of a membership fee(for a challenge, the attacker can try to enroll as a prime member without actually paying the membership fee).
  </li>
  <li>
   <b>Photo Wall and Tweet Button</b>
   : Many online vendors allow users registered as sellers to upload images and users registered as buyers to upload images and videos online on a photo wall or as reviews to a product. As the images are directly uploaded without sufficient checks, the application becomes susceptible to various vulnerabilities.
  </li>
</ol>

#### Why did I choose this idea for the project?
When I first browsed the Juice Shop idealist the idea seemed to be very interesting and fun in the sense that I was allowed to think features without any restriction and implement them.

<br>

As a user of the Juice Shop, I always felt the need of a few features such as a payment gateway and an order history page. I also thought it would be nice to have features such as privileged membership and a wallet which is a growing trend in the e-commerce presently. This motivated me to pursue the project right from the moment I saw it.

#### Challenges

There were times during the GSoC period where I faced various challenges but I was able to complete it with research, consistency but most importantly with the guidance of my mentors, who were always there for me throughout the GSoC page for which I am grateful. I learned a lot from them, and it was an extremely great experience to work under their mentorship.

#### Thanking Note

I extend my sincere gratitude to all readers for taking the time to read this report. I would also like to thank everyone who helped me in contributing to the project and honing my skills.
