# Vue-Select-image
A clean and simple Vue component allowing for selection of images from list. Works well on small and large projects , and supports all 4 language models and the full Vue stack.

# WEB-Vue-Select-image

![Project Logo](/assets/robot.gif)

**WEB-Vue-Select-image** is a Vue.js component that enables image-based selection within a web application. This component allows users to choose an image from a predefined set of options and provides a callback function to handle the selected image.

## Features

- Single image selection from a list of options.
- Displays selected image and accompanying message.
- Simple integration into Vue.js projects.

## Demo

A live demo of the component can be found ~~[here](https://openco.ca/vue-select).~~ NOTE: currently down.

## Installation

The installation steps for integrating WEB-Vue-Select-image into your Vue.js project are as follows:

1. Clone the repository:
   ```
   git clone https://github.com/your-username/WEB-Vue-Select-image.git
   ```

2. Navigate to the project directory:
   ```
   cd WEB-Vue-Select-image
   ```

3. Include the component in your Vue.js project by importing it where needed:
   ```javascript
   import ImageSelect from "./components/ImageSelect.vue";
   ```

4. Use the component within your Vue.js template:
   ```html
   <ImageSelect :dataImages="dataImages" @onselectimage="onSelectImage"></ImageSelect>
   ```

5. Customize the component as per your application's requirements.

## Usage

To use the WEB-Vue-Select-image component in your Vue.js application, follow these steps:

1. Import the component in your Vue file:
   ```javascript
   import ImageSelect from "./components/ImageSelect.vue";
   ```

2. Add the component to the `components` property of your Vue instance:
   ```javascript
   components: {
     ImageSelect
   }
   ```

3. Define the necessary data and methods within your Vue instance:
   ```javascript
   data: function() {
     return {
       dataImages: [
         // Define your image options here
       ],
       // Other data properties
     };
   },
   methods: {
     onSelectImage: function(image) {
       // Handle the selected image here
     }
   }
   ```

4. Use the component within your Vue template:
   ```html
   <ImageSelect :dataImages="dataImages" @onselectimage="onSelectImage"></ImageSelect>
   ```

## Customization

The WEB-Vue-Select-image component can be customized to suit your application's visual style. The CSS classes provided in the component's `<style>` section can be modified or extended to achieve the desired appearance.

## Contributing

Contributions to WEB-Vue-Select-image are welcome! If you encounter any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/opencoco/WEB-Vue-Select-image/issues).

## License

This project is licensed under the GNU Affero General Public License (AGPL). Please see the [LICENSE](/LICENSE) file for more information.

## Credits

- [Vue.js](https://vuejs.org/) - JavaScript framework for building user interfaces.

## Contact

For any inquiries or further information, please contact [your-email@example.com](mailto:info@openco.ca).

---

*Note: This README template does not include installation instructions and assumes the project is published under the AGPL.*
