### Adding a New Section

1. **Add a Button:**
   - In the `<div id="homepage">`, add:
     ```html
     <a class="btn btn-primary random-position" href="#<section-id>" id="<section-id>-btn" onclick="showSection('<section-id>')"><Section Name></a>
     ```

2. **Create the Section:**
   - Add this below the other sections:
     ```html
     <div id="<section-id>" class="container section">
       <button class="btn btn-secondary back-btn" onclick="goBack()">Go Back</button>
       <h1><Section Name></h1>
       <div class="row">
         <div class="col-md-6">
           <img class="mx-auto d-block" src="path/to/<section-image>.jpg" alt="<Section Name> Image" style="width: 100%; max-width: 200px; margin-top: 20px;">
         </div>
         <div class="col-md-6 text-md-start">
           <br>
           <p>Content for the <Section Name> section goes here.</p>
         </div>
       </div>
     </div>
     ```

3. **Create Button for the Section:**
   - In the script, update the `buttonTitles` array:
     ```javascript
     const buttonTitles = ['who', 'canada', 'work', 'blog', '<section-id>'];
     ```

4. **Verify Navigation:**
   - Ensure `showSection` and `goBack` functions are implemented and work correctly.

5. **Test:**
   - Open the HTML file in a browser.
   - Verify the new button navigates to the new section and the "Go Back" button returns to the homepage.
