# ParaModular-Spool-Holder
A parametric and modular spool holder that fits any spool width, and can also be extended!

*Please excuse me for my horrendous renders!*
<img width="751" height="793" alt="Render Main" src="https://github.com/user-attachments/assets/99beb8c0-f97b-43ec-91e5-e540912edefb" />


### Introduction
This is the paramodular spool holder, a completely parametric spool holder which can also be extended with magnets and screws.

Its features include:
- Completely parametric settings for Spool length and width, along with other parameters to change the holder itself (*see configurations*)
- A removeable and customisable label for labelling your spools
- Toggleable magnet and screw holes to allow for modularity with other spool holders

My idea for this was to replace simple store bought boxes and crates with something that had the sole purpose of storing filament spools, with some added functionality.

### Model
The design includes 2 main parts: the label, and the holder itself which are printed separately.

Here you can see the complete assembly, with a standard 1kg spool added for reference:
<img width="563" height="790" alt="Front" src="https://github.com/user-attachments/assets/912829c2-1766-4313-b042-af03eff1cd97" />

The label simply slides into a slot at the front of the holder which allows for a relatively loose fit. This is done so that it can be easily interchanged.
<br><br><br>
The spool itself sits on 2 grooves running along the holder, this should allow the spool to sit comfortably without falling out easily:
<img width="812" height="726" alt="Side" src="https://github.com/user-attachments/assets/96f7a988-a5d6-4118-84ce-aa766be5a8ea" />
<br><br>
You can also add magnet and screw holes to the holder to make it modular. The way this works is by having magnets on one side and screws on the other, so if you print 2 of the same holder then the magnet side of one holder will be attracted to the screw side of the other. This allows you to make a chain of holders that you can also easily take apart.  

Here is what one of the magnet holes looks like on the model:
<img width="774" height="677" alt="Magnethole" src="https://github.com/user-attachments/assets/53fd372e-fd21-445a-8d2c-8cc127aca088" />

The magnet's size is configurable, and it should press fit into the hole with a clearance of 0.1mm. It's also a good idea to put a little superglue into the hole before pressing in the magnet. 
<br><br><br>
Here are one of the screw holes, directly opposite to the magnet holes on the other side of the holder:
<img width="1059" height="764" alt="Screwhole" src="https://github.com/user-attachments/assets/031603be-ca50-4df5-9a9e-a7b9eee36cec" />

The screw's dimensions are also configurable, but the point is that the screw's head should lay flush with the recessed wall of the holder.

### Configurations
The holder was modelled in fusion 360 so I have set up customisable user parameters for each major dimension. These are also included in the configuration menu where you can make your own presets or use mine.

Here is what the user parameters look like in the model parameters:
<img width="1862" height="578" alt="UserParameters" src="https://github.com/user-attachments/assets/3c15b21c-faac-4755-adc6-28a933ee9cff" />

Here is a table which clearly describes each parameter, its function, and some recommended dimensions:
| Name | Default Value | Comments |
|---|---|---|
| Spool_Diameter | 200 mm | Diameter of your spool |
| Spool_Width | 67 mm | Full width of your spool |
| Spool_RimWidth | 3.5 mm | Width of one of the rims of your spool |
| Holder_Thickness | 10 mm | Thickness between the spool and outer wall of the holder (Recommended 10mm) |
| Holder_Height | 90 mm | Height of the holder from the bottom (Recommended Max: Spool Diameter / 2) |
| Lable_Width | 55 mm | Width of label (Recommended Max: Spool_Width - 1mm) |
| Label_Height | 45 mm | Height of Label (Recommended: Holder_Height / 2mm) |
| Label_Title | PLA | Title text for label |
| Label_SubTitle | 190°C – 210°C | Subtitle text for label |
| Label_TitleHeight | 15 mm | Height of title text on label |
| Label_SubTitleHeight | 5 mm | Height of subtitle text on label |
| Row_ArrayNumber | 1 | Changes the amount of holders in one row. Adjust based on print volume (Will not copy labels) |
| Holder_FilletSize | 25 mm | Changes the size of the fillet on the bottom of the holder |
| Magnets Toggle | OFF | (**Availiable in configurations**) Toggles whether to include magnet/screw holes for modularity |
| Magnet_Diameter | 6 mm | Diameter of your magnets |
| Magnet_Height | 3 mm | Height of your magnets |
| Screw_ThreadWidth | 3 mm | Width of the threads on your screws or simply the "M" number (eg. M3) |
| Screw_HeadHeight | 2 mm | Height of the head of your screws |
| Screw_ThreadLength | 8 mm | Length of the threads on your screws |
| Screw_HeadWidth | 5 mm | Width of the head of your screws |

The default values shown here are the ones from my preset for a 1kg spool
<br><br>
Here are 2 configurations I've made as an example of how you can use these parameters:


1. A heavy-duty 300mm spool holder with magnets
<img width="1113" height="664" alt="ConfigEx1" src="https://github.com/user-attachments/assets/3e0aebb0-e032-453b-81a8-89c73159f666" />
<br><br>
2. A double, 100mm spool holder also with magnet slots
<img width="1343" height="788" alt="ConfigEx2" src="https://github.com/user-attachments/assets/cecb1962-3a92-4b0d-a932-56b79ad14d93" />

### Print Settings
In the CAD folder I have also included a ready to print 3mf of my 1kg spool preset which should (hopefully) fit a single 1kg spool.
Here are 2 general tips if you are planning to print your own configuration:

1. Print orientation - Orientate the holder on its side with the protruding magnet holes facing up (if you have them included), making sure that the angled part of the label slot is also the one on top. The label should then be placed flat on the print bed with the text facing up.
<img width="888" height="693" alt="PrintOrient" src="https://github.com/user-attachments/assets/e1a7530d-f5fe-4b50-9940-c0cf8ab0944e" />
<br><br>
2. Counterbore hole bridging - Enable this option in your slicer if you have the magnets option enabled in your configuration. Otherwise, the recessed holes for the screws will create a counterbore hole that cannot be printed easily. Enable this option to "partial" or "partial bridge" which will simply print an extra bridge or two below the hole which can be removed after printing.
<img width="746" height="623" alt="Counterbore" src="https://github.com/user-attachments/assets/5f2f57d4-3c16-4c9b-8e86-3b15fba51580" />

### BOM
| Part | Vendor | Cost/item | link | Estimated Dicounted Price |
|---|---|---|---|---|
| 6x3mm Magnets | AliExpress | $5.88 | [AliExpress](https://www.aliexpress.com/item/1005010074888189.html?spm=a2g0o.productlist.main.8.7d1722940e6u9q&algo_pvid=d8094d71-d422-4f77-a95e-1cace47c2982&aem_p4p_detail=20261017122917458118601081260003689373&algo_exp_id=d8094d71-d422-4f77-a95e-1cace47c2982-7&pdp_ext_f=%7B%22order%22%3A%225532%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21NOK%2172.37%2133.70%21%21%2149.12%2122.87%21%4021613ab217922653569711158e10aa%2112000051279728372%21sea%21NO%218463637778%21X%211%210%21n_tag%3A-29911%3Bd%3A22d43e35%3Bm03_new_user%3A-29895%3BpisId%3A5000000220090510&curPageLogUid=dKp6xIkZyOTM&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005010074888189%7C_p_origin_prod%3A&search_p4p_id=20261017122917458118601081260003689373_2) | $2.74 |
| M3x8mm Screws (**Self Provided**) | AliExpress | $0 | (Example Link) [AliExpress](https://www.aliexpress.com/item/1005006938221639.html?spm=a2g0o.productlist.main.2.45f92330G0PhRg&algo_pvid=45187495-7f33-4ca8-b2f8-aaed3f47222c&algo_exp_id=45187495-7f33-4ca8-b2f8-aaed3f47222c-1&pdp_ext_f=%7B%22order%22%3A%221947%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21NOK%2111.71%218.19%21%21%217.95%215.56%21%400b884a9917923340672134917e0dad%2112000038790430953%21sea%21NO%218463637778%21X%211%210%21n_tag%3A-29911%3Bd%3A22d43e35%3Bm03_new_user%3A-29895&curPageLogUid=8Kw4b3Tqk1NT&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005006938221639%7C_p_origin_prod%3A) | - |
| Shipping + Tax |  | $4.97 |  | - |
| Total |  | $10.85 |  | $7.71 |

Here $5.88 represents the **maximum possible price** of the item, discounts are shown in right column and in cart screenshots

The model itself will be printed on my own printer so no price has been added

Cart Screenshots (1kr ≈ $0.1):

<img width="777" height="193" alt="Cart Screenshot" src="https://github.com/user-attachments/assets/0645a1b0-5af9-43f5-97a6-28ea6550869f" />

<img width="378" height="309" alt="Payment Screenshot" src="https://github.com/user-attachments/assets/f7a782c3-85e3-465f-86f7-f9844a913373" />
