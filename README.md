STEP-1:Create a Lex with HotelBookingBot

STEP-2:Create a role with basic Amazon Lex permissions

STEP-3:Select none in the voice interation

STEP-4:Add a inten name

STEP-5:In sample Utterances add Utterance metioned in document

STEP-6:Navigate to slots tab

STEP-7:Open location slot add location in name and add What city will you be staying in? in promts. check the required for this intent

STEP-8:Open nights slot add nights in name and add How many nights will you be staying? in prompts

STEP-9:Add new slot with name checkinDate and What day do you want to check in? in prompts and SAVE INTENT & BUILD

STEP-10:Navigate to slot types and add a blank slot type named roomtype

STEP-11:Select restrict to slot values in roomtype slot and add Queen,King,Delux,superDelux and save

STEP-12:Go back to the BookHotel intent add room type slot and  add What type of room would you like , Queen,King, Deluxe and Super Deluxe?

STEP-11:In prompts.SAVE INTENT & BUILD

STEP-13:In confirmation prompts add Okay,I have youn down for a {Nights} night stay in{Location} starting {CheckInDate}.Shall I book the reservation? and select okay i have cancelled your reservation in declined response

STEP-14:In fullfillment goto adwanced options add thanyou in messagegroup and click update options SAVE INTENT & BUILD

---------------------------------------ATTACHING BOT TO LAMBDA---------------------------------------------------------

STEP-1:Create a fuction with Python3.9 as Runtime

STEP-2:Configure the testevent

STEP-3:Now open Aliases option in AWS Lex

STEP-4:Select TestBotAliases and in language select English add lambda in SOURCE

STEP-5:Now open BookHotel intents in below select click use a lambda for intialization SAVE INTENT & BUILD

STEP-6:Update the Given python code in Lambda and Deploy

STEP-7:Build & Test the HotelBooking Intent

--------------------------------------CREATING TWILIO ACCOUNT-----------------------------------------------------------

STEP-1:Buy a Number with SMS capabilities

STEP-2:Navigate to AWS Lex console

STEP-3:Create a new version in Bot Versions

STEP-4:Create a New Aliase(hotelbotaliase) and associate with before created version

STEP-5:ADD CHANNEL in Channel Integrations Add Twilio SMS  & add hotelbotaliase & add TWILIO SID,AUTHENTICATION CODE

STEP-6:Copy callback URL in Channel intergration

STEP-7:Navigate to TWILIO account

STEP-8:Messaging >Try it Out >send a watsapp message

STEP-9:Complete Twilio sandbox & watsapp setup

STEP-10:After completion Twilio sandbox setup paste callback URL copied from Channel intergration and SAVE

⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡THANKIN YOU⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡⚡
