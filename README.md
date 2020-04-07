# Export assets from Adobe XD
 
## Introduction
We created an integration tool for you to integrate your design assets easily from [Adobe XD](https://www.adobe.com/products/xd.html) to [Respresso](https://respresso.io). Let's see how to use it perfectly.
 
## Usage
Create a project in Adobe XD and create your app's design. Finally, import the design assets into Respresso with Adobe XD plugin.
 
## Integration settings
 
 #### Server address
	
 Basically, it is https://app.respresso.io. Change this address if you have an own Respresso server.
 
 #### Project token
	
Respresso has a project token for importing data from outside tools. This token isn't the same with your project token.  You will find this token in the path of Project settings/Integration options.
	
 #### Export mode
This is a simple option to choose a comfortable way of exportation. You can export all of your artboards or only the selected items.
	
#### Localization
Plugin will export your localization strings if you leave the tick in the rect. These texts have a key and value pair inside XD. Value is a simple text that you can write into a textbox. Key is more complicated than value. You will find this under the Layers window. Click on the textbox and check the Layer. In that you can modify the key with a double click on the textview with a T symbol. Respresso suggests a key usage like these:
	
* section.name_of_the_function.name_of_element (main.menu.log_out)
* section_name_of_the_function_name_of_element (main_menu_log_out)
* connected_to.function_name_of_element (user.log_out)
* etc.
	
<p align="center"><img src="documentation/localization.png"></p>
 
Sometimes designers have to modify localization inside the designer tool. We are motivated to help you and for developers that is why you can reimport all of your localization texts. Let's see how we handle it.
 1. Modifying the value is the simplest case. Respresso will follow the modification.
 2. Key modification not acceptable function through import. Respresso will skip this request. 
 3. Remove isn't acceptable as well.
 
 Sometimes you would like to skip some texts. In that case add this command: #respresso-ignore to the text's key field.
	
#### Color
Respresso plugin can export all of your colors from Color Assets. Export all of your colors from artboards not an option, please use Color Assets. Respresso supports solid and gradient colors, although gradient colors will split by parts of colors and Respresso exports them like solid colors. Colors Assets supports key and value pairs. You can modify the key of the color with double click on the color under Colors section.
 
<p align="center">
	<img src="documentation/color_add.png">
	<img src="documentation/color_assets.png">
</p>
 
Respresso supports the modification of the color. Change the value and reimport the project. Key modification not supported.
	
#### Image
You can export all of your images from Adobe XD with a simple solution. Select an image and tick Mark for Export option under Appearance section on the right. Respresso supports vector and raster formats but we would like to suggest svg type. Images have keys as well and you can modify it in the assets window. Click the Layers icon on the left bottom position. Select an image from an artboard and Adobe XD will select the item in the windows. Use double click on the item and you can rename it.
 
<p align="center">
	<img src="documentation/export.png">
	<img src="documentation/image_rename.png">
</p>
 
Change your image asset or add a new one export option. Image modification is fully supported. 
	
#### App Icon
Create your app's icon(s) in Adobe XD. Respresso plugin supports Simple and Background - Foreground icons. To import app icons into Respresso you have to tick the Mark for Export option under the Appearance section on the right and use specific keys for images.
* Singe icon key: App icon single
* Background icon: App icon background
* Foreground icon: App icon foreground
 
Modification is supported as well.
 
## Integration config
 
Configuration windows show basic information about a team and project. You can select a version for each digital asset, which was selected previously. 
 
## Change Log
 
Change log contains all modifications (create or update) about the project. This may help you to follow the import process.
