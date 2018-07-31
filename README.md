# Fire-Plane-FB-Reactions
For Those asking How to Do Plane/Fire Reaction :

1. Create a new Bookmark

2. 

• Name : Anything you want (example : FB Reactions)

• URL : Copy/Paste code below

```
javascript:let hookFacebookReactionsCounter=0;function hookFacebookReactions(){const modulesToHook=['UFICentralUpdates','UFIFeedbackTargets'];const updateFeedbackEvent='update-feedback';const defaultReactionsCount=6;const newReactions=[{name:"fire",id:14},{name:"plane",id:15}];if(window.requireLazy){window.requireLazy(modulesToHook,(UFICentralUpdates,UFIFeedbackTargets)=>{UFICentralUpdates.subscribe(updateFeedbackEvent,onUpdateFeedback);function onUpdateFeedback(eventName,feedbackObj){var supportedReactions=feedbackObj.feedbacktarget.supportedreactions;if(supportedReactions.length===defaultReactionsCount){for(let reaction of newReactions.reverse()){supportedReactions.push(reaction.id)}
feedbackObj.feedbacktarget.supportedreactions=supportedReactions;UFICentralUpdates.inform(updateFeedbackEvent,feedbackObj)}}});let cssText=``;for(let reaction of newReactions){cssText+=`div[data-reaction='${reaction.id}'] div._4sm1:after { content: ' ${reaction.name}'; }`}
let hookScript=document.createElement("style");hookScript.type="text/css";hookScript.textContent=cssText;(document.head||document.body||document.documentElement).appendChild(hookScript)}else{console.log('Failed to inject Facebook Reactions hook.');hookFacebookReactionsCounter++;if(hookFacebookReactionsCounter<30)setTimeout(hookFacebookReactions,50)}};hookFacebookReactions()

```

3. Save and Click on Home link

4. TADAAAA... That's all 😉

Star this if you like it ⭐
