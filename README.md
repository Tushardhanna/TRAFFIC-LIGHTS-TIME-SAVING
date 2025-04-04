# TRAFFIC-LIGHTS-TIME-SAVING
Manages the time of the traffic light depending upon the length of the traffic in each lane
CODE 
import random

def chatbot_response(user_input):
    responses = {
        "hello": "Hi! How can I assist you with smart traffic lights?",
        "how does it work": "The system uses sensors or cameras to detect the number of vehicles in each lane and adjusts the traffic light timing accordingly.",
        "benefits": "It reduces congestion, minimizes wait times, and improves fuel efficiency by optimizing traffic flow.",
        "technology used": "The system can use AI, computer vision, and IoT sensors to analyze and control traffic signals dynamically.",
        "implementation challenges": "High costs, integration with existing infrastructure, and data privacy are some of the challenges.",
        "bye": "Goodbye! Drive safe!"
    }
    
    return responses.get(user_input.lower(), "I'm not sure about that. Can you ask something else?")

# Example conversation
while True:
    user_input = input("You: ")
    if user_input.lower() == "exit":
        print("Chatbot: Goodbye!")
        break
    print("Chatbot:", chatbot_response(user_input))
