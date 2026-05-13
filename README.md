# FunkyStation-Medical-Suggestions  
These changes shouldn't slow down medical gameplay too much. 
 
They keep the current damages and treatments: Players getting 1 of the 5 types of damages during the game still get the same treatment that everyone knows.
 
People who tick some medical records in the customization window will get extra content and RP potential. For others, nothing changes. This new content should be easy to go through (1 condition has 1 treatment that should be taken regularly, usually a pill, and can lead to a complication if untreated, which will deal 1 of the 5 type of damage). For example, untreated asthma leads to an asthma attack, which deals `asphyxiation dmg`.  Some severe conditions should crit patients (stroke).

There should be a book (like the chef's recipe book) that shows which treatment is required for which disease, and what potential complication it can have. Interns could spawn with it, or it could be located somewhere in the medbay.  

Names of real molecules will be provided. It should help the players that are familiar with some of them, or people working in healthcare. This document adds a lot, so it would be easier for medbay staff without fictional names. Or maybe change the names to fit the NT lore? This is a design choice not up to me.
  
There are also suggestions regarding existing medical tools, like stethoscope, and possible new ones (EKG, reflex hammer, x-ray). These tools should not be required to use, but they should provide small clues and fun content when roleplaying. 

This documentation will try to provide accurate real-life (IRL) information, followed by how it could be implemented in a basic way ingame, in order for developers to make the right choice balance/complexity wise.  
   
I hope this make the game more interesting for medical and non medical crew on the station.  
   
## Add a personnal medical history (most is already ingame as "Family Medical History").  
 
The `Personnal medical history` will define what condition players have currently, and which treatment they should spawn with. Each condition, if left untreated, can lead to a complication and damages.  

Some of these would be too complicated to show ingame and could be not interesting, some have no impact on gameplay but can be kept for RP reasons.  

|Name|What it is|How it could be done ingame|Treatment|Complication if missed treatment|
|---|---|---|---|---|
|Allergies (non food, see at the bottom for food allergies)| Allergies against certain allergens floating around in the air. Happens a lot in places that are not cleaned, and in spring with trees and flowers|Janitor could be useful. It should trigger in places with dust and stains on walls, or due to touching some materials like latex in some gloves. Get  `skin rash` on basic health check, `itches` a lot, `sneezes` a lot. See below for food allergies.|Antihistamines|None ingame 
|Anemia|Low red blood cell count, has many causes but iron deficiency is the most common|Less tolerance for bleeding (faster `bloodloss dmg`?), `pale skin` all the time, and `tired` when running?|IRL : Too many different causes and treatment. Ingame: no treatment? Or get an IV bloodpack at the medbay and it's fixed for the whole round?|It's more of a long term chronic health issue. Nothing should happen ingame.
|Anxiety|self explanatory|Get `stuttering` or `shaking`, and "*feeling anxious*"|Solved by taking pills when the first signs appear|Get a `panic attack` and stay frozen for a few seconds
|Arthritis|Joints getting old and painful|Get `pain`often especially while moving|Standard painkillers (paracetamol) available at the pharmacy|None|
|Arrhythmia|Irregular heartbeats, with fast exhausting heart rate for severe cases. You can hear it with a stethoscope, and see it on an EKG| "*You start to feel irregular heartbeats...*".|Antiarrhythmics (Flecainide) prevents it|`Arrhythmia`with : `exhaustion`, fast irregular heartbeats showing with EKG and stethoscope? or on the HealthAnalyzer? Needs fast IV Amiodarone OR Defib to cure. Leads to cardiac arrest (`aphyxiation dmg`) if left untreated too long and death.
|Asthma|Difficulty breathing due to hypersensitive bronchi. Triggered by viruses, pollutants in the air, and sometimes a physical effort|`gasps` if `allergens` in the air, running too long, or has a cold/flu (upcoming virology?). Cannot run for a while|Beta-2-Agonist (Salbutamol) inhaler stops all symptoms|"*It's very hard to breath*" after a while, `crit`and `Asphyxiation dmg`|
| Auto-immune (AI) disorder|The immune system is a bit trigger-happy and can damage various cells of the body (AI thyroid disease, Type 1 Diabetes, etc.)|Too many AI diseases to count, so no ingame effect, purely RP.|None|None ingame|
|Blood clots|Blood clots block veins and arteries (more dangerous)|Clot in vein: `pain` and sometimes swollen limb. Clot in artery:`pain x2`and no pulse, cold and grey limb.|Bloodthinners prevent them, the most famous being warfarin (used to cure too, but let's not make it too complicated).|Kinda complicated? Vein clot =`pain` only. Clot in artery: `brute limb dmg` going up fast + `pain`. IV Heparin (stronger) to cure, in medbay. Clots can also move and reach the heart/lungs arteries which is a pulmonary embolism (very dangerous, can lead to cardiac arrest), and brain (stroke), but probably doesn't need to be in SS14.|
|Cancer|A cell started to disobeys the self-kill signals, and multiplied...|RP only|IRL chemotherapy, radiotherapy, surgery|None ingame|
|Chronic pain (rename to something more specific: back pain?)| self explanatory| Get `pain`often|Standard painkillers (paracetamol) available at the pharmacy|None|
|Depression|self explanatory (often linked with anxiety)|`cries`and `sighs`often?|Antidepressants (sertraline). All of them are long term treatment. But for game reasons we could give them instant effects? Or maybe get round length symptoms if you forget to take them one time? (text prodroms should alert the player to take pills in that case)| None ingame|
|Diabetes|Sugar stays in the blood instead of going in the cells (often due to lack or lesser sensitivity to insulin, a hormone that makes it go in the cells)|See below (lot to say about this, would be complicated but could make chef gameplay more interesting)
|Essential tremor (New)|Hands and fingers become shaky especially while using them (writing or drinking with a glass). Can affect vocal cords|Shaky hands and drop items on the ground regularly|Betablockers|None
|Heart disease (Rename to chronic heart failure)|The heart is not as good at pumping blood as it used to be|Get `tired` faster when running.|Beta-blockers (propranolol)| `Acute Heart Failure`with : `Oedema`, `shortness of breath` and `asphyxiation dmg` (shows on basic health check), cannot move much. Stethoscope would show crackles when listening lungs (because water goes in). Requires diuretics (IV furosemide, medbay) that makes you pee and lowers the load on the heart.|
|High blood pressure|self explanatory|Add an item to measure ingame? or show numbers on the HealthAnalyzer? Normal values are around 130/75 mmHg.|Antihypertensives|`pain`("*has a headache*") if above 170/110. The same treatment should make it go back to normal (IRL it sometimes needs IV antihypertensives in the ER).|
|HIV|A virus that slowly disables the immune system over years|RP only (or maybe in upcoming virology? Viruses evolves and spread faster). Syringes can maybe contaminate others... Use autoclave to clean.|IRL antivirals|None ingame|
|Insomnia (New)|Self explanatory|RP only|Sleeping pills (interesting for antags. Can be put into food/drinks)|None
|Kidney disease (Rename to chronic kidney disease)|The kidney does not remove toxics and salt that you eat as good as it used to. Most treatment's dosage needs to be adjusted for people with renal failure (lower dose). At the final stage, natural pee volume is greatly reduced and dialysis is needed.|RP only? (complicated topic, has lots of ways it could be implemented). Maybe just lower the treshold for drug overdose as they are not filtered out of the blood as fast?|No treatment, IRL we only manage to slow it down by lowering high blood pressure if there is, high sugar level if there is (those damage kidneys over time). Dialysis in hospital regularly when it's very bad.|IRL : Acute renal failure. Ingame : implant new kidney and take immunosuppressives ? Tbh it could just lower treshold for OD and that's it.|
|Liver disease| There are a lot of liver diseases (infectious, auto-immune, alcohol...)|RP only| None|None|
|Lung disease|Same|RP only|None|None|
|Migraines|A special kind of headaches. Often inherited from a parent.|"*You remember it's time to take your migraine treatment*"|Beta-blockers only prevent migraines. |Get`pain`("*has a pulsating headache*"), sometimes `nausea`and `light sensitivity`. Standard painkillers (paracetamol) to cure, available at the pharmacy|
|Neuroaversion|Not something medical, but Ive seen it used in the codebase with migraines, not sure what it does.|
|Organ transplant (New)|Self explanatory||Immunosuppressives|Organ failure (would require to copy paste this condition for all possible ingame organs so we know which one fails)
|Osteoporosis|The bone mineral density is low. For elders mostly. Bones are weaker|RP only? Take blunt damage faster? Fractures system needed? See below|
|Schizophrenia|Psychiatric conditions involving hallucinations, negative symptoms (flattened affect, restricted range of emotions)|Might start seeing monsters instead of players, hear weird noises or voices.|Antipsychotics|None ingame
|Seizures (rename to Epilepsy)|Epilepsy is a condition that can trigger seizures. Some parts of the brain, usually the cortex, are more sensitive to stimuli.|Epilepsy often doesn't have symptoms (except a few specific types), only seizures, when they happen.|Antiepileptics|`Seizures` : Character shaking on the floor for up to a minute. Leads to `asphyxiation dmg`if it lasts too long. Usually `very tired` when waking up. Can be stopped instantly with IV midazolam (anticonvulsivant).
|Sleep Apnea|You stop breathing, multiple times, for a few seconds at night without knowing, blood O2 decreases and then goes back to normal. Often gives high blood pressure during the day.|RP only|IRL : a machine that gives pressurized air through a mask during sleep, or a mouth guard that pulls the jaw forward at night|None
|Stroke|A brain artery gets a blood clot. Blood stops flowing in that area of the brain. The risk of getting a stroke is much higher if one already happened. Bloodthinners can be prescribed after a stroke, to prevent new ones.|RP only|Bloodthinners|Another clot (see above) or stroke: Various symptoms (one to multiple) : not being able to use a hand ingame, standing on feet (one leg paralysis), everything heard or spoken appears ingame as gibberish (aphasia), one side of the vision is gone (either left or right side of the game screen = hemianopia). See below for picture. Gives `asphyxiation dmg`? Or no dmg but should crit and kill after a timer. Treated in medbay with IV t-PA (Alteplase), the strongest thrombolytic.
|Reflux|Sometimes, the stomach content goes up and is very acid and burning|Get `chest pain` and "*burps*"|Antiacids pills (omeprazole)|None in game


There are medications that could be dangerous for some :  
Blood thinners : Do not give to someone already bleeding! Makes bleeding 2 times faster. Some use case for blood cult?  
Beta-blockers can trigger an asthma attack for those with asthmatic condition.  

It would be interesting to try to communicate with the patient, as some conditions change stuff (e.g. OD treshold for chronic kidney disease)

## Diabetes system 
 Maybe to work on last? Would require lot of dev work:  
 Ingame implementation: Add sweetness level to meals (1-5), and blood sugar level to HealthAnalyzer (normal, high, very high) After eating, the blood sugar level should go up (value depends on what food the chef gives you. A salad gives you 1, whole cake gives you 5. At 5 you reach the coma stage (requires IV insulin at medbay). Taking medication before eating prevents blood sugar level from rising, and diabetic coma.  
 Pro : Funny things might happen around the kitchen. Interesting topic to talk about with the Chef. More variety in food because of health issues.  
 Cons : Lot of work only for people who would tick diabetes medical record. The Chef already has a lot to plan around.  


## Fractures system
All 4 limbs can be fractured. More chances of giving someone a fracture using a blunt weapon, and aiming on limbs.  
To treat a patient, put him in a medbed. (Optional : IRL, need an x-ray machine to see if the fracture has moved or if all fragments are aligned. Or, physical exam  could otherwise show if the fragments seem aligned or not). If needed, right clic the patient in the bed and "align the fracture" (very painful! use some morphin beforehand otherwise it adds some brute damage). Take a cast, clic on the sink to put water on it, and clic on the patient. It will apply on the fractured limb. Once the fracture is consolidated (xray could show that if ingame), the cast can be removed (right click or add a cast cutter tool into the game).  
Can be balanced however the team wants: If a leg is fractured, the player can move with crouches (uses both hands)? If both legs are fractured the player can only move in a wheelchair? (would require lot of sprite work I guess for every angles, races, and clothes. Render characters in wheelchair with hospital gown for simplicity?). Or everyone can walk but slowly? Cast should last a short time ingame (15min?) and then good to be removed at the medbay.  

	
	
## Prescriptions given at round start according to player's `personnal medical history`:
---------------------------------------
	Antiacid pills for reflux (omeprazole)
	Antiarrhythmic pills for arrhythmia (flecainide)
	Antidepressant pills for depression (sertraline)
	Antiepileptic pills for epilepsy (levetiracetam)
	Antihistamine pills  for allergies cetirizine)
	Antihypertensive pills for high blood pressure (irbesartan)
	Anxiolytic pills for anxiety (alprazolam)
	Antipsychotic pills for schizophrenia (quetiapine)
	Antithromboti pills for strokes (acetylsalicylic acid) : Work a bit differently than bloodthinners. 
	Beta-2-agonist inhalers (Salbutamol) for asthma
	Beta-blocker pills for chronic heart failure, migraine, essential tremor (propranolol)
	Bloodthinner pills for blood clots and strokes (warfarin).
	Hormone pills (Too many, should be removed, keep as a personal medical history only : Keep just for RP or remove? Lot of  things based on which hormones. Probably unnecessarily complex. May or may not fit the game based on politics. See below.
	Immunosuppressive pills for organ transplant patients (mycophenolate mofetil)
	Insulin pen (New) : There are other oral drugs for diabetes but this one is the most famous (insulin pens or syringes). Could be used on people that don't have diabetes to incapacitate them temporarily and even kill them (coma and asphyxiation dmg).  
	Painkiller pills (paracetamol)
	Sleeping pills (zopiclone) : should not be carried during the shift as you don't sleep during daytime, it could look suspicious based on the context, unless you're heading to a consultation where the doc will ask your medical history, or to pharmacy, or other reasons!
	
A limit of health conditions a player can have should be set, for gameplay reasons.  

Patients should take their meds regularly if prescribed. Otherwise, their condition may worsen (see above).  

"Taking meds regularly" should be set to a an amount of time, but I don't know yet. 30 min ingame? Check shift time in PDA? 

Meds should be pills of various colors. Some should be IV for the most severe conditions, and cannot be self-administered. See below for new IV drugs.  

Keep `family medical history` for RP.  

Some players should spawn without their meds (Patients often cannot get an appointment fast enough to renew them, or forget them when travelling). This would lead to more early shift gameplay for doctors, with a few patients coming in to renew their prescriptions (RP).


Having these various conditions and prescriptions would lead to interesting RP with CMO or attending physiciaan doing rounds for interns?

  ## Newly introduced medbay IV drugs 
---------------------------------------
	Amiodarone : A strong IV antiarrhythmic that stops arrhythmia.
	Furosemide : An IV diuretic that heals acute heart failure. Makes you pee and lowers the load on the heart.
	Heparin : An IV bloodthinner that heals severe cases of blood clots.
	Insulin : Should be available in IV therapy in medbay for people in diabetic coma (after eating too many sweets or food without prior insulin pen injection).
	Midazolam : A strong IV anticonvulsivant that stops seizures.
	rt-PA (Alteplase) : The strongest thrombolytic, used for strokes to get rid of the clot very fast.





  ## New, or expanded medical tools
---------------------------------------
	Defib : Wake people up from cardiac arrest. Used also on arrhythmia patients instead of IV Amiodarone.
	Stethoscope : Should show both heartbeats (regular, or fast and unregular for arrhythmia) and respiratory sounds (normal respiratory sounds, or crackles for acute heart failure)
	Reflex hammer : Add a hammer that can be used on limbs to show increased reflex response  (from the stroke). Can be used if insure of diagnosis, or for RP. *the arm/leg shakes normally* or *the arm shakes a lot and multiple times*
	Blood presssure monitor : Used to check the BP of patients. Used in high blood pressure. More RP that ways instead of simply showing numbers during the health check.
	EKG : Roughly the size of the crash cart. Needs EKG paper and one cell. Links to a patient in a bed in the same way as the IV stand. Interact with it to print the paper. Paper, when used, should show a floating text with the diagnosis to doctors, and a text with "complicated lines" to non medical crew. Shows a flat line when used on a dead patient.
	Cast: Used for fracturess. Clic on the sink to put water on it, and clic on the patient. It will apply on the fractured limb. Once the fracture is consolidated, remove with a cast cutter.
	Cast cutter: A circular electric saw roughly the size of the hand labeler used to cut casts. Requires a cell.
	X-ray machine : Should be the size of a medbed. Drag and drop someone inside. The picture is triggered behind a shield in order to avoid radiations. The room should be closed. Anyone standing around should get radiations when triggered.
  
I think the most important ones to begin with are the defib and stethoscope changes, and the hammer for fun (easy to do).


## Allergies : 

Limit to food to begin with (airloss dmg + skin symptoms), then extend in the future to materials (latex etc. with checks when handling different items; and skin symptoms only)  

Meals should have a gametag containing allergens they has been made with (milk, nuts, wheat etc).  
Perform a check with player's allergies when eating.  

If allergic : skin rash and itchiness, stomach pain, diarrhea after a while (brown puddle on the ground? janitor with hazmat gameplay! can be avoided by going to toilets?). Can trigger an airway oedema (character gasps, asphyxiation dmg) : Epinephrin pen heals it.  

Patients should know their allergies. It could also be shown in the medical record terminal in the medbay.  


# Pictures and explanations
Example of hemianopia during a stroke : 
<img width="163" height="192" alt="hemianopia" src="https://github.com/user-attachments/assets/621be6c5-93c6-43b7-a6ed-1cafcee4bd7f" />
<img width="236" height="220" alt="hemianopia2" src="https://github.com/user-attachments/assets/d79c88a2-a80b-44d8-97e9-118ffbf559c9" />


![Example of hemianopia during a stroke.](https://my.clevelandclinic.org/-/scassets/images/org/health/articles/homonymous-hemianopsia-2)



To rephrase or make more clear :
shouldnt slow down medical gameplay.
People getting 1 of the 5 types of damage around the space station still get the same treatment as usual.
People who tick some medical records in the customization will get more content and RP. This content should be easy to go through (1 condition has 1 treatment usually a pill, can lead to getting 1 of the 5 type of damage if untreated.
The expanded usage of existing items such as stethoscope is not mandatory to use. Use if you are unsure to get more clues, or use for RP.

