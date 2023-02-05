# ChatGPTWizard
<b><h2>This is an OpenAI (ChatGPT) plug-in for Embarcadero RAD Studio IDE.</h2>
<h2>First, you need an API key that you can generate here: (https://beta.openai.com/account/api-keys)<h2>
<br><h2>Remarks</h2>

1. It is compatible with Xe5 and later versions.
1. Uses XSuperObject library which is included in the project files.
1. Settings are stored in registry which can be found here: Computer\HKEY_CURRENT_USER\Software\ChatGPTWizard
1. Consider that if you run it in the IDE without opening any project it will raise a message that it cannot load the SSL library
1. This issue can be fixed if you put SSL libraries(can find them in the resource folder) besides the bds.exe or in Bpl folder(mine is this ==> C:\Users\Public\Documents\Embarcadero\Studio\22.0\Bpl)
or you can use a build event on the project's properties to copy these two class libraries if there are not.
Another point: You don't have to do that because it will work fine when you open any project in the IDE before using this plugin! I'm not sure that this behavior depends on the installed components or libraries or if the IDE will load SSL libraries at the moment you open even a new application, although using the plugin when you are working on a project seems more useful anyway.</h3>

<h3><b>How to install</b></h3>
 Open the project, right-click on the project in the project manager, build, and install.  
  
<h3><b>How to use</b></h3>

1. you can use the ChatGPT menu from the IDE's main menu directly to ask questions and get the answer.
Click on the newly added ChatGPT menu on the IDE(or press Ctrl+Shidt+Alt+C) to open the wizard, type the question and press the Ask button(or Ctrl+Enter).
![image](https://user-images.githubusercontent.com/5601608/215458671-a48a4e1d-3b2c-45bd-9da5-603ab82129dc.png)

1. If you need to use the ChatGPT inside the editor you need to make(type) a question directly inside the code editor and surround it with "cpt:" at the beginning and ":cpt" at the end of the question then press Ctrl+Shift+Alt+A or simply select "Ask" from the editor's context menu by right-clicking on the selected text.

1. Use the "ChatGPT Dockable" menu from the main menu to show the dockable form and try to dock the form to the left or right side panel of the IDE, and enjoy with your new Google killer assistant!

![image](https://user-images.githubusercontent.com/5601608/215994463-2b24cea1-aea4-4d35-9beb-ea795edbc76d.png)


<br><h2>Simple Test scenario</h2>
Open a new vcl applicatiopn project, add a new unit and remove all the code from it! and type the following line, select all and press Ctrl+Shift+Alt+A.<br>
<b>cpt:Create a full unit in Delphi including a class to create an XML file.:cpt<b>
 ![image](https://user-images.githubusercontent.com/5601608/215461813-7ecf4555-b3a2-4c0e-b85e-6069ead6a3d9.png)

Demo video 1 : https://youtu.be/vUgHg3ZPvXI
<br>Demo video 2(full demo): https://youtu.be/rQgh63DXGoE <br>

Presentation: [CHAtGPT wizard.pptx](https://github.com/AliDehbansiahkarbon/ChatGPTWizard/files/10612086/CHAtGPT.wizard.pptx)

<br>Goud luck.
