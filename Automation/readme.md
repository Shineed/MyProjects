This is the read file to explain how I have done the scenario

I have used Selenium, Java and TestNG framework to code this program. 

Before starting the test, it will open the chrome browser and enter the url once the browser get maximised.

Then, for Test, identified the elements to enter the text in search box and click the search icon.
Once the page navigates to result page, then I Select parent element of Best Seller Product and avoid duplicate/repeat product.
While the best seller product has itself a hyperlink page to navigate, I select the href attribute using stream().map(Function) from best seller element.
Iterate the best seller to navigate and add to cart. So each href page will open and add to cart and again navigate the next one and add to cart till the iteration ends.

As part of validation, get the text of proceed to check out and validate the count of products added with the count of href attribute
