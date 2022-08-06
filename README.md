# Overview
The single API call is made in the `App` component

## Description
### Product Overview:
It has 4 main parts:
1. Image Gallery: displays product images and includes and an expanded view interactions to zoom into a selected image.
2. Product Information: displays a star rating, product category, title, price
3. Style Selector: interactive thumbnails for each style of the product. Selecting a style will change change the related images and available sizes.
4. Add to Cart: Two dropdowns that allow the user to select the size and quantity of the item to add to their cart. The options available within these dropdowns will vary based on the selected product style.

  
  
### Related Items & Outfit Creation:
It has 2 main parts:
1. Related products: 
    - This component displays a carousel of product cards that are related to the product currently being viewed. 
    - Each product card renders the images, category, name, price and star rating. 
    - By clicking the star action button on cards, it will open a comparison modal comparing the characteristics of the product of the current page to those of the product that was selected from the list.
    - By default, the preview image displayed on each card is the same which first appears on the image detail page’s image gallery. 
    - Users can view additional preview images by hovering over the initial preview image that appears on the card. 
    - Users can change the preivew image by clicking on a thumbnail in the preview image carousel.

2. Your Outfits: 
    - Your outfit: displays products which the user selected and marked as their favorite outfits. The list items persist across page navigation.
    - The first card on the left hand side of the list acts as a button to add the currently viewed product to the outfit list.
    - The concurrent product cards will look similar to the ones in Related Products. The 'X' button on the cards allow users to remove the product from the outfit list.
  
### Ratings & Reviews: 
The Ratings & Reviews module will allow viewing and submission of reviews for the product selected. It has 5 main parts:
1. Reviews List: 
    - It displays a list of all the reviews that have been submitted for the product being viewed. By default, the list only display 2 product tiles at a time. By clicking "More Reviews" button to load more reviews. 
    - Each review tile displays the following information: start rating, reviewer name, date, summary, body, recommend, response to review, rating helpfulness.
    - For each review, user can cast a vote for the helpfulness or report a review. User can make one submission for each review. 
2. Write new review: 
3. Sorting: users can combine the following options to sort the review list.
    - Sort by sort drop down options: helpful, newest, relevant
    - Sort by star rating
5. Rating Breakdown: display each of the star ratings that a customer gave to this product.  
6. Product Breakdown: Feedback for characteristics will be displayed on a 5 point scale.
7. Keyword search: user can filter the reviews for any that contain text matching the search term in the search bar.


# Setup

1. Create a file `config.js` file. Make sure to add it to your `.gitignore`
2. Create a cloudinary token (for image uploading)
3. Below is the need format for the `config.js` file. `Token` refers to the API token.
  ```
  module.exports = {
    cloudinaryInfo: {
      cloud_name: '',
      api_key: '',
      api_secret: ''
    },
    token: ''
  }
  ```
4. Run the following commands in your terminal: `npm install`, `npm run server-dev`, `npm run react-dev`
5. open `http://localhost:3000/` in the browser.




