I have used TestNG framework to code this program. SO before starting the test, it will intialise the browser and enter the url once it get maximised.

Then, for Test, I have identified the elements to enter the text in search box and click the search icon.
Once the page navigates to result page, then I Select parent element of Best Seller Product and avoid duplicate/repeat product.
While the best seller product has itself a hyperlink page to navigate, I select the href attribute using stream().map(Function) from best seller element.
Iterate the best seller to navigate and add to cart. So each href page will open and add to cart and again navigate the next one and add to cart till the iteration ends.

As part of validation, I have just get the text of proceed to check out and validate the count of products added with the count of href attribute
