###SOA Microservice API

Microservices architecture is an alternative approach to structuring applications. An application is broken into smaller, completely independent components, enabling them to have greater agility, scalability, and availability. SOA exposes the functions of applications as more readily accessible service interfaces, making it easier to use their data and logic in the next generation of applications.

Imposible to gain agreement. Their definitions have a lot of room for interpretation

An SOA appears to have an enterprise scope, where applications communicate with one another. An SOA exposes services through standardized interfaces between applications. The microservices architecture appears to have an application scope, with a focus on the structure and components within an application.

SOA is based on two views that address two different needs

***

#### An over-simplified view

The reason that it is difficult to compare SOA and microservices is that their definitions have a lot of room for interpretation. If you have only a surface-level knowledge of the two concepts, they can sound similar. Key aspects, such as componentization, decoupling, and standardized communication protocols, describe most software initiatives in the last few decades, so we need to dig deeper.
Consider the following simple definitions:

###### Microservices architecture

is an alternative approach to structuring applications. An application is broken into smaller, completely independent components, enabling them to have greater agility, scalability, and availability.

###### SOA

exposes the functions of applications as more readily accessible service interfaces, making it easier to use their data and logic in the next generation of applications.
An SOA appears to have an enterprise scope, where applications communicate with one another. An SOA exposes services through standardized interfaces between applications. The microservices architecture appears to have an application scope, with a focus on the structure and components within an application.

These definitions of SOA and microservices are too simplistic. In fact, the relationship between them is much more complex.

***



##### Dichotomy of SOA initiatives

When you look at an SOA in more detail, you can see that its original intent was broader than exposing interfaces as SOAP web services. SOA is based on two views that address two different needs.

###### Integration-led technical element
The first view encompasses the need to integrate deep into existing systems over their complex and often proprietary data formats, protocols, and transports. Then, the need is to expose them by using standardized mechanisms (such as SOAP/HTTP or more recently JSON/HTTP) to make them easier to re-use in new applications. This view is shown on the left side of Figure 2. Some or all of this view is often referred to as an Enterprise Service Bus (ESB) pattern. However, this term is used indiscriminately to the point of making it meaningless.
The need to do deep integration (integration hub and adapters) and to expose these integrations as services or APIs in a standardized way (exposure gateway) is essential. This aspect has everything to do with integration challenges and little to do with application design. Consequently, therefore, it appears to have little relationship with the microservices application architecture.


###### Business-led functional element

The second view is from a business perspective. The concern is that the interfaces on the current systems are largely meaningless. They don't make sense to the business, and they don't provide what's needed for the next generation of applications. They might be too granular, exposing too much of the complex data models within the systems. The data that is required might be spread across multiple systems. The data models might not resemble the terminology that is used by the business.
The need entails functional refactoring to expose something that the business can tangibly build into future solutions. This refactoring requires the creation of new applications to bind together requests across the existing systems of record. In the SOA reference architecture, these applications were often referred to as service components. This view shows a relationship to application design (and, therefore, the microservices architecture) and the functional decomposition of capabilities into separate components.

###### The challenge of mixing the views

Organizations vary in which of the two views is the greater challenge. For some organizations, their greatest challenge is the diversity and complexity of the integration. For others, refactoring and relandscaping to achieve the right business functionality is the primary challenge. Figure 2 shows how different the problem can look, depending on which of these two challenges is forefront in your mind.
For many, the challenge is a painful mixture of both views. It is painful because it's difficult to merge the two views into a single course of action. Integration tools are not the right place to perform business logic. Conversely, you do not want your business applications to be cluttered with technical integration concerns.
The goal of most SOA programs is to achieve the functional aspects. They want easily accessible business-relevant services that can be used to build new applications more effectively. However, many run out of momentum, or more commonly out of budget, while still solving technical integration challenges. In large enterprises, SOAs are often perceived to have failed. This thought might be true in that they failed to deliver the final business value, although huge strides were made to improve the accessibility of systems of record. However, in smaller companies (or more contained environments within larger companies), SOAs often claim true business successes because they can quickly overcome integration issues and move on to functional benefits.
These two views of SOA make comparisons with microservices challenging.


#### How APIs compare to SOA exposed services

APIs used to mean low-level programming code interfaces. In recent years, the term has been reappropriated to mean simple interfaces provided over HTTP. Typically, it equates to REST interfaces, which provide data by using the JSON data format (sometimes XML), and the HTTP verbs PUT, GET, POST, and DELETE to depict create, read, update, and delete actions. These protocols and data formats are simpler to use than the web services standards based on SOAP that were more prevalent in early SOA. Also, they are more suited to such languages as JavaScript that are commonly used when making API requests.
However, the difference between SOA web services and APIs isn't defined by protocols and data formats because they are not used consistently between the two. The difference lies in the intent behind APIs and SOA services. One key difference is in their economics.

###### The reusable SOA


###### The dawn of API management


#### Microservices: An alternative architecture

Before you look at a comparison of microservices and SOA, you need to understand what a microservices architecture means. From a fundamental point, microservices are an alternative architecture for building applications. They offer a better way to decouple components within an application boundary. In fact, if microservices were called "micro components," their true nature would be clearer.
The boundaries of the application remain the same. As shown in Figure 4, despite being broken into separate microservice components on the inside, the application might still look the same from the outside. The number and granularity of APIs that a microservice-based application exposes should not be any different than if the API was built as a siloed application. The prefix "micro" in microservice refers to the granularity of the internal components, not the granularity of the exposed interfaces.





