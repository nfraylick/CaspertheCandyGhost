##Casper, the Candy Ghost

## Inspiration
We want Halloween, so we hacked a way to keep everyone safe with Casper. We wanted to create something that will positively impact the community and allow people to feel safe enough to participate in Halloween. By using incentives, like candy, people will be adherent to the Covid-19 guidelines by requiring them to wear a mask.

## What it does
When someone comes up to Casper, the AI detects if they are wearing a mask and dispenses candy into their bag.   

## How we built it
We use a machine-learning algorithm and OpenCV on a Raspberrypi with a camera to determine if someone is wearing a mask. We created our own Haar Classification by taking pictures of our team members with and without masks on. To train the AI more, we also uploaded pictures from the internet of people wearing their masks. This allows the AI to pick up on more details and have a higher percentage of certainty when determining if the individual is wearing a mask or not. If the individual is wearing a mask, then the candy dispenser is put into a state where candy can be dispensed. The data from the Raspberrypi is then sent to our local server. In the local server, we compile the data and display the status of Casper as well as stats like the number of people who came, the number of people wearing a mask and no mask, etc. The server then transmits the data from the server to an ATMEGA328P microprocessor that is attached to an ESP8266 wifi module. Once the data is sent to the ATMEGA, the micro waits until a bag is detected under the machine. This fully automated process keeps people safe by having a hands-free way of delivering candy and also encourages people to adhere to Covid-19 policies.

## Challenges we ran into
This was our first time developing an AI and our first time using a Raspberrypi. Most of the time early on was taken up by installing everything we needed to develop this project. OpenCV was giving us problems where it wanted different dependencies to properly install. We had to look up how to use facial recognition and how to train the AI to detect faces and masks.

## Accomplishments that we're proud of
We developed our own AI! We have never used python for such a big project like Casper. We used a lot of hardware to gather data and a load of software to compute and interpret the data.

## What I learned
We had a tough time setting up our hardware to behave the way we wanted to, but we learned what was needed to be installed prior to the. We learned how to create our own Haar classification to determine if an individual is wearing a mask or not.

## What's next for Casper, the Candy Ghost
We hope if Halloween is not canceled for 2020, we would like to use this in our neighborhood to ensure everyone is safe having fun.
