---
name: Immunize
tools: [Figma]
image: https://res.cloudinary.com/valentinesalim/image/upload/v1615882199/SAVE_LIFE_SAVE_TIME_iavrjn.gif
description: Mass vaccination effectively, efficiently, and safely.
---

{% include elements/video.html id="eod8dyC2WTI" %}
## Inspiration

When the first experimental COVID-19 vaccine became available in China, hundreds of people started queuing outside hospitals, waiting to get that vaccine. Imagine this on a planetary scale when the whole everybody has to be vaccinated all around the world. There's a big chance while queuing they can spread the virus to people around them or maybe get infected because they cannot perform social distancing at all. We sure don't want that to happen.

The other big issue is that there are lots of conspiracy theories, rumors, stigma, and other forms of disinformation simultaneously spread across our social media about COVID-19 and it's vaccine. This misinformation creates frustrations for users many asking, we really don't know which one is right? Which one is wrong?

## What it does

Immunize is a mobile app that can save your life and save your time. The goal is to make the distribution of mass-vaccination become more effective, faster, and less crowded. With this app, you can book your vaccine appointment based on your own preference. So the user can easily choose the hospital based on the nearest location and easily schedule an appointment based on their availability.

In addition, based on the research we found that most of Covid-19 vaccines requires 2 doses given in 3 weeks apart to achieve that high effectiveness. And there's a big probability that people can forget to return for a follow-up shot. We can minimize that probability. This app will automatically schedule the patient for the 2nd vaccination so there is a less likelihood of user error. The reminder system (as notification feature) that will remind them in their phone when they have appointment that day.

## How we built it
We built the prototype using flutter as our client to support mobile. We integrated radar.io for hospital search. For facial recognition we used GCP and SMS reminders we used twilio. The mobile client connected to firebase: using firebase for auth, firebase storage for avatars and firestore for user metadata storage. The second backend host used datastax.

## Challenges we ran into
Working with an international team was very challenging with team members 12+ hours apart. All of us were learning something new whether it was flutter, facial recognition or experimenting with new APIs. Flutter APIs were very experimental, the camera API had to be rolled back two major version which occurred in less than 2 months to find a viable working version compatible with online tutorials

## Accomplishments that we're proud of
The features:

1. **QR Code Feature** for storing all personal data + health condition, so user don't need to wait for a long queue of administrative things.

2. **Digital Registration Form** checking if user is qualified of COVID-19 vaccine and which vaccine suits best.

3. **Facial Recognition** due to potential fraud in people who are not eligible for vaccination attempting to get limited supplies of vaccine, we implemented facial recognition to confirm the user for the appointment is the same one that showed up.

4. **Scheduling Feature** based on date, vaccine availability, and the nearby hospital.

5. **Appointment History** to track all data of patients, this data can be used for better efficiency of mass-vaccination in the future.

6. **Immunize Passport** for vaccine & get access to public spaces. This will create domino effect for people to get vaccine as soon as possible so that they can get access.

7. **Notification** to remind the patients every time they have appointment/ any important news via SMS and push notifications

8. **Vaccine Articles** - to ensure the user can get the accurate information from a verified source.

9. **Emergency Button** - In case there are side effects after vaccination.

10. **Closest Hospitals/Pharmacies** - based on a user's location, users can get details about the closest hospitals through Radar.io Search API.

## What we learned
We researched and learned a lot about the facts of COVID-19 Vaccine; Some coronavirus vaccines may work better in certain populations than others. And there may be one vaccine that seems to work better in the elderly than in younger populations. Alternatively, one may work better in children than it works in the elderly. Research suggests, the coronavirus vaccine will likely require 2 shots to be effective in which taken 21 days apart for Pfizer's vaccine and 28 days apart for Moderna's remedy.


## What's next for Immunize
Final step is to propose this solution to our government. We really hope this app could be implemented in real life and be a solution for people to get COVID-19 vaccine effectively, efficiently, and safely. Polish up our mobile app and build out an informational web app and a mobile app for hospital staff to scan QR codes and verify patient faces (currently they have to use the same app as the client)

## Preview
![alt text](https://res.cloudinary.com/valentinesalim/image/upload/v1615882255/Immunize_mockup-min_entwey.jpg)
