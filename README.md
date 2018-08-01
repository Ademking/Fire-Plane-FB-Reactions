# Fire - Plane Facebook Reactions 🔥🛩

![](https://i.imgur.com/7r1JzwS.gif)

For Those asking How to Do Plane/Fire Reaction :

# Chrome :

1. Create a new Bookmark

![](https://i.imgur.com/BFoalbL.png)

2. Fill the bookmark :

![](https://i.imgur.com/aCxdeK2.png)

• Name : Anything you want (example : FB Reactions)

• URL : Copy/Paste code below

```
javascript:let hookFacebookReactionsCounter=0;function hookFacebookReactions(){const modulesToHook=['UFICentralUpdates','UFIFeedbackTargets'];const updateFeedbackEvent='update-feedback';const defaultReactionsCount=6;const newReactions=[{name:"fire",id:14},{name:"plane",id:15}];if(window.requireLazy){window.requireLazy(modulesToHook,(UFICentralUpdates,UFIFeedbackTargets)=>{UFICentralUpdates.subscribe(updateFeedbackEvent,onUpdateFeedback);function onUpdateFeedback(eventName,feedbackObj){var supportedReactions=feedbackObj.feedbacktarget.supportedreactions;if(supportedReactions.length===defaultReactionsCount){for(let reaction of newReactions.reverse()){supportedReactions.push(reaction.id)}
feedbackObj.feedbacktarget.supportedreactions=supportedReactions;UFICentralUpdates.inform(updateFeedbackEvent,feedbackObj)}}});let cssText=``;for(let reaction of newReactions){cssText+=`div[data-reaction='${reaction.id}'] div._4sm1:after { content: ' ${reaction.name}'; }`}
let hookScript=document.createElement("style");hookScript.type="text/css";hookScript.textContent=cssText;(document.head||document.body||document.documentElement).appendChild(hookScript)}else{console.log('Failed to inject Facebook Reactions hook.');hookFacebookReactionsCounter++;if(hookFacebookReactionsCounter<30)setTimeout(hookFacebookReactions,50)}};hookFacebookReactions()

```

3. Save and Click on Home link

4. TADAAAA... That's all 😉

--------

# Firefox :

1. In Firefox, click "Bookmarks," then select "Bookmark this Page"

![](https://mreidsma.github.io/bookmarklets/img/firefox2.png)

2. Type a name for your bookmarklet into the Name field, and select where you want the bookmark to live. If you want it easily accessible, choose the "Bookmarks Toolbar."

3. You should have a bookmark in your toolbar now. Right-click on it and select "Properties."

![](https://i.imgur.com/QyAxuPb.png)

4. Copy/Paste the JavaScript code below for your bookmarklet, and paste it into the "Location" field.

```
javascript:let hookFacebookReactionsCounter=0;function hookFacebookReactions(){const modulesToHook=['UFICentralUpdates','UFIFeedbackTargets'];const updateFeedbackEvent='update-feedback';const defaultReactionsCount=6;const newReactions=[{name:"fire",id:14},{name:"plane",id:15}];if(window.requireLazy){window.requireLazy(modulesToHook,(UFICentralUpdates,UFIFeedbackTargets)=>{UFICentralUpdates.subscribe(updateFeedbackEvent,onUpdateFeedback);function onUpdateFeedback(eventName,feedbackObj){var supportedReactions=feedbackObj.feedbacktarget.supportedreactions;if(supportedReactions.length===defaultReactionsCount){for(let reaction of newReactions.reverse()){supportedReactions.push(reaction.id)}
feedbackObj.feedbacktarget.supportedreactions=supportedReactions;UFICentralUpdates.inform(updateFeedbackEvent,feedbackObj)}}});let cssText=``;for(let reaction of newReactions){cssText+=`div[data-reaction='${reaction.id}'] div._4sm1:after { content: ' ${reaction.name}'; }`}
let hookScript=document.createElement("style");hookScript.type="text/css";hookScript.textContent=cssText;(document.head||document.body||document.documentElement).appendChild(hookScript)}else{console.log('Failed to inject Facebook Reactions hook.');hookFacebookReactionsCounter++;if(hookFacebookReactionsCounter<30)setTimeout(hookFacebookReactions,50)}};hookFacebookReactions()

```

5. Save and Click on Home link

6. TADAAAA... That's all 😉

--------

# Safari

Dragging the link to the bookmarks bar is the easiest way to do this in Safari. Otherwise we have to create a bookmark for something else, and then edit the URL to be the Javscript we want to run.

1. In Safari, open https://facebook.com

2. Select Bookmarks > Add Bookmark

3. A little window will pop up. Select the folder or location where you want the bookmarklet (Use "Favorites Bar" for easy access.) Then type the name of your bookmarklet in the text field. for this example write "Facebook Reactions"

4. Click "Add"

5. Now right-click on bookmark you just created. You should see a menu pop up. Select "Edit Address"

![](https://mreidsma.github.io/bookmarklets/img/safari1.png)

6. You should now see a text box pop up under your bookmark

7. Copy/Paste the code below :

```
javascript:let hookFacebookReactionsCounter=0;function hookFacebookReactions(){const modulesToHook=['UFICentralUpdates','UFIFeedbackTargets'];const updateFeedbackEvent='update-feedback';const defaultReactionsCount=6;const newReactions=[{name:"fire",id:14},{name:"plane",id:15}];if(window.requireLazy){window.requireLazy(modulesToHook,(UFICentralUpdates,UFIFeedbackTargets)=>{UFICentralUpdates.subscribe(updateFeedbackEvent,onUpdateFeedback);function onUpdateFeedback(eventName,feedbackObj){var supportedReactions=feedbackObj.feedbacktarget.supportedreactions;if(supportedReactions.length===defaultReactionsCount){for(let reaction of newReactions.reverse()){supportedReactions.push(reaction.id)}
feedbackObj.feedbacktarget.supportedreactions=supportedReactions;UFICentralUpdates.inform(updateFeedbackEvent,feedbackObj)}}});let cssText=``;for(let reaction of newReactions){cssText+=`div[data-reaction='${reaction.id}'] div._4sm1:after { content: ' ${reaction.name}'; }`}
let hookScript=document.createElement("style");hookScript.type="text/css";hookScript.textContent=cssText;(document.head||document.body||document.documentElement).appendChild(hookScript)}else{console.log('Failed to inject Facebook Reactions hook.');hookFacebookReactionsCounter++;if(hookFacebookReactionsCounter<30)setTimeout(hookFacebookReactions,50)}};hookFacebookReactions()

```

8. Click the "Done" button.

![](https://i.imgur.com/nKapR7K.png)

------

# Press That Star Button if you like it ⭐

![](https://i.imgur.com/gtVE2rx.png)
