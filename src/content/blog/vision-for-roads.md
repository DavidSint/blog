---
title: 'A Vision For Roadway Infrastructure'
description: 'Explore the future of roadway infrastructure, envisioning smarter and safer roads as well as more efficient and pleasurable driving experiences for all.'
pubDate: 2024-06-17
heroImage: '../images/blog-smart-roads.png'
---

On long drives, I often contemplate how we could improve road infrastructure, particularly if we were to build it from scratch today with an unlimited budget. In the UK, we have been building _smart motorways_, which have been controversial due to the removal of the _hard shoulder_—the lane used for emergencies. These projects operate within limited budgets and are cautious about future vehicular technology, resulting in motorways designed for the present rather than the future.

Instead, let's explore a concept for our roadways that does not heavily consider cost, feasibility, or budget constraints, similar to how concept cars showcase potential features that may eventually enter production models.

## Principles & Assumptions

To ground this concept in reality, we need some guiding principles:

1. Ensure backwards compatibility with non-smart vehicles (progressive enhancements and graceful degradation).
2. Include redundancies as technical failures are inevitable.
3. Utilise vehicles as sensors where possible, rather than relying solely on bespoke sensors.
4. Assume not all cars will be autonomous.
5. Assume not all cars will be electric.
6. Assume legislation can ensure vehicular manufacturers comply with interoperability standards.

## The Concepts

### Network Participants

The system comprises:
1. Centralised system
2. Signage and gantries
3. Communication mesh network
4. Road users

<div class="scroller">

| Participant | Description | Examples |
| --- | --- | --- |
| **Centralised system** | Stores the accurate state of the network, responds to information requests, and communicates with other network nodes like signs and road users. | Data centers, cloud infrastructure |
| **Signage** | Displays information to non-smart vehicles. | Gantries, standalone signs |
| **Communication mesh network** | A P2P communication network with a dedicated waveband and senders/receivers on the roads, and vehicles | Gantry antenna, camera antenna, vehicle antenna |
| **Road users** | These have sensors and are able to communicate with the network. | Cars, vans, lorries, cyclists |

</div>

### Digital Twin and Signage

All roads and infrastructure should be stored as a digital twin in the centralised database. When events such as breakdowns or hazardous road conditions occur, they should be digitally tagged on the road.

Most road signage should be digital to some degree. Fixed signage, such as alerts for road curves, is unnecessary to digitise as vehicles will have this information from their mapping data. However, if information cannot be inferred from standard in-built systems, the road infrastructure should relay this information to the network or have it tagged in the centralised system. For instance, if a road is prone to icy conditions, this should be tagged and shared with road users as a warning.

Digital twins also enable predictive maintenance of roads. Using the existing sensors on the roads, vehicles and using the data e.g. number of weather cycles and vehicles on a certain patch of road, authorities can predict maintenance and schedule repairs at opportune times.

### Communication and Integration

#### Shared Communication Language

It is essential for network participants to communicate using a shared language. All network nodes should communicate with vehicles, the road network nodes, and the central system. This communication should function like a mesh network, where vehicles can use other nodes to communicate. For example, a car unable to get a signal can relay a message through other vehicles to report an issue.

#### Hazards, Road Conditions, and Alerts

Imagine a system where vehicles' sensors and sat-nav systems detect hazards and road conditions in real time. This data can be sent to the network, logged in the digital twin database, and displayed on digital signage or sent directly to vehicles. The network would provide continuous updates on traffic conditions, weather hazards, accidents, and other relevant information, allowing vehicles to alert drivers or adjust routes accordingly.

In the event of a crash, other vehicles and road sensors would send this information to the centralised service which could coordinate the response effort with emergency responders.

#### Local-First Communication System
The communication system should prioritise local communication before escalating to broader networks. This approach starts with logging an event internally, extends to vehicle-to-vehicle or vehicle-to-road using a specific band for peer-to-peer (P2P) communication, and finally to vehicle-to-cloud using a vehicle's SIM or a connected mobile device. This ensures updates are saved and eventually reach the central system directly or through peers.

Events from nodes will require de-duplication and a consensus algorithm to align on an accurate road picture. This algorithm can be iteratively improved for precision. The centralised architecture will simplify the consensus-building process compared to more complex public blockchain algorithms.

#### Data Schema for Interoperability

A standardised data schema would allow vehicles to understand and react to conditions and messages. Instead of dictating specific actions (e.g., switch to a snow-specific mode), the system alerts the vehicle to the current condition (e.g., it's snowing), and the vehicle or driver decides the best course of action. This flexibility ensures a wide range of vehicle types and technologies can integrate and innovate without limiting potential options.

### Communication Channels

Communication between vehicles, the road, and central systems should use multiple channels to ensure robustness and redundancies:

1. **Vehicle SIM-based Communication**: For vehicles that are internet connected and when there is good cellular coverage.
2. **Mobile connected Communication**: Piggy-back off of the connected phone in the vehicle to use that internet pathway in areas with good coverage.
3. **P2P over Dedicated Band**: For direct communication between vehicles and roadside senders/receivers.
4. **Networked Charging Lane**: Similar to Scalextric, these lanes can power/charge vehicles and provide data transfer capabilities.
5. **Gantry/Signage**: For fallback and redundancy, ensuring information is always available even if other channels fail.

### Autonomous and Non-Autonomous Lanes

Once autonomous vehicles are significantly safer than human drivers, dedicated lanes for autonomous vehicles could have higher speed limits due to increased safety. These lanes would facilitate smoother traffic flow and encourage the adoption of autonomous driving technologies. Non-autonomous lanes would operate at standard speed limits, ensuring safety for all road users.

Speed limits for autonomous vehicles would be variable based on road conditions, such as lower limits when approaching bends and higher limits on straight sections.

Different lanes could also cater to different driving preferences. For instance, a dedicated slower lane for those prioritising efficiency or reducing motion sickness, and a faster lane for those in a rush.

Further, because these lanes are autonomous, depending on traffic conditions and time of day, the centralised system can dynamically convert a lane to go in the other direction to reduce congestion. The system can also clear a lane just ahead of an emergency response vehicle when it is responding to an alert.

### Centralised System and Offline Archives

The centralised system would maintain an archive of road data, providing valuable insights for future system improvements and policy-making. By analysing traffic patterns, accident data, and road conditions, authorities can make informed decisions to continuously improve roadway infrastructure and safety standards.

## Conclusion
Envisioning modern roadway infrastructure from the ground up demonstrates what's possible. By integrating a digital twin system, a dedicated communication network, and smart vehicle technologies, we can significantly enhance the safety and efficiency of our roads. Emphasizing principles like backwards compatibility, redundancy, and interoperability ensures a smooth transition from current vehicles while encouraging adoption of smarter technologies. Ultimately, this concept envisions a roadway system where digital and physical realms converge, fostering a safer, smarter, and more responsive driving environment for all.
