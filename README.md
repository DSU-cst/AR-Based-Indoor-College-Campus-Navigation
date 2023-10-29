
# Augmented Reality Based College Campus Indoor Navigation

While GPS is widely used for outdoor navigation, it falls short indoors. While some maps are available on campus, users do not receive continuous assistance to reach their destinations. They may attempt to plan their routes using these static maps, but once they begin walking in their intended direction, they lack ongoing guidance. Indoor navigation often requires expensive additional hardware. This project explores techniques for indoor campus
positioning, pathfinding, and route guidance. Our project's goal is to introduce a cost-effective indoor campus navigation system. Our solution utilizes the built-in sensors in mobile devices to pinpoint user location and combines them with AR technology to provide an immersive navigation experience.

## Problem Statement

● Navigating inside campus, particularly for
newcomers, is challenging due to limited guidance
and the absence of effective navigation systems.

● Need for a AR based navigation experience for
better visualization and understanding of the route
compared to 2D Maps or boards.

## What our Project does ?

● Our project aims to create an affordable and
user-friendly indoor Campus navigation system by
utilizing the sensors in mobile devices.

● We will develop a mobile apk that integrates with
AR Foundation for precise indoor positioning and
ARCore for real-time AR guidance.

● Users will have the option to choose their desired destination within the campus, and they will receive AR-based navigation to enhance their visual user experience.

### Literature Survey

The following link contains the Literature survey's of few research papers related to this project - 
https://docs.google.com/document/d/1QqfRV16re0NvfmY8iGACqnWsCJHELwkcPTNeZt0ApgU/edit?usp=sharing

## Design

There are three stages in this project

<img src="https://github.com/CapstoneProjectDSU/Augmented-Reality-Based-indoor-College-Campus-Navigation/assets/149241928/c36bd865-d831-4510-acfc-ed32a1ebc695" width="320" height="500">
<br></br>

i) **Mapping** - Campus indoor floor is designed and the 3D environment is created using Unity. The attributes and scaling must be accurate.

ii) **Localization** - There are various ways to detect the user location without the help of GPS such as :

● Beacons - A Bluetooth beacon is a small wireless device that works based on Bluetooth Low Energy. These are small devices which need to be purchased and placed all over the campus. It helps to calculate the user location and guide them accordingly. (Accuracy - 5 meters)

    Pros - Easy setup
    Cons - Expensive and not feasible inside campus.

● Visual positioning system (VPS) - Uses smartphone camera to analyze the surrounding and determine user location

    Pros - Automated and accurate.
    Cons - It is complicated to set up and configure. We need create our own datasets 
           and train artificial intelligence models to recognize environments.

● Visual Markers - It is an image which the system can recognize. It must be a unique and asymmetric image so that the system can understand from which side it is viewing the marker.

    Pros - Highly accurate and easy to set up.
    Cons - Periodic rescanning.

We use Visual Markers technology in our project since it is cost effective and highly accurate. 
Visual markers are helpful for ensuring IPS (indoor positioning system) accuracy. Each marker has its own unique ID. These markers tell the user's position in 3d space.

iii) **Visualization** - Visualization is about presenting information to the user in an understandable and intuitive manner, combining the digital and physical worlds.

● AR Rendering: Use AR Foundation to render AR content, such as directional lines, blips, or labels, in the user's view based on their position and the target location.
● Minimap Display: Create a minimap that shows an overview of the indoor environment and indicates the user's position and the target location as blips.
● UI Elements: Design and display user interface elements for start and target selection, navigation controls, and any feedback.

In this visualization stage, we provide the user with an AR-enhanced view that guides them from the start point to the target point, incorporating elements like directional lines, minimaps, and user interface components.

## AR Based Campus Indoor Navigation Architecture 

![IndoorNavArchitectureDiagram](https://github.com/CapstoneProjectDSU/Augmented-Reality-Based-indoor-College-Campus-Navigation/assets/149241928/a9fd980d-4d0f-4649-a1ea-e2a14903ccd3)




