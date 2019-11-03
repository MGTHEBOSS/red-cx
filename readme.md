## Red CX

The customer experience management market will be worth [$14.5 B](https://www.marketsandmarkets.com/PressReleases/customer-experience-management.asp) in 5 years. [72%](https://www.slideshare.net/ekolsky/cx-for-executives) of customers share a good experience with at least 6 people. [30%](https://www.investopedia.com/financial-edge/1010/top-6-reasons-new-businesses-fail.aspx) of new businesses fail in the first 2 years, 50% in the first 5 years, and 66% in the first 10 years. A principal reason a business fails is due to its inability to ensure a good experience for customers. If we take a website for an example, if a customer does not get what they want, they are going to leave the site in a short time, and not only that, they are going to talk about their bad experience in social places, for instance, in coffee shops, shopping malls, bars etc. or on facebook, twitter, instagram etc. What they say is going to influence other customers. If 4 out of 5 colleagues of a person say a product is bad, that person will not be very interested in purchasing the product. Every customer directly or indirectly influences the experience of other customers. 

Probability is a fascinating concept that has been under-exploited in the customer experience domain. The [classical definition of probability](https://www.encyclopedia.com/science/encyclopedias-almanacs-transcripts-and-maps/probability-basic-concepts-mathematical-probability) says, "If there is a finite number of possible outcomes of an experiment, all equally likely and mutually exclusive, then the probability of an event is the number of outcomes favorable to the event, divided by the total number of possible outcomes." Red CX is a probabilistic inference based customer experience engine that calculates the probability of all customers having a good experience. The user needs to enter the no. of customers and then the required probability values. The solution will then calculate the probability of all customers having a good experience. It is based on the chain rule of conditional probability i.e. P(∩ k=1 to n CK)=Π k=1 to n P(CK|∩ j=1 to k-1 CJ). For instance, in order to calculate P(C1∩C2∩C3), it will require the values of P(C1), P(C2|C1), and P(C3|C1∩C2). When entered, the value of P(C1∩C2∩C3) will be calculated and displayed to the user. 

It has been built using leading web technologies. At its core, it's a node app. It uses a redhat application runtime. It's hosted on the redhat openshift container platform. It's secured using redhat single sign-on (SSO). It has 2 deployments, 1 for the app (1 pod) and the other one is for sso (1 pod). It has 1 provisioned service, redhat single sign-on 7.2 ephemeral. The app build's source is the github repository. The app has 2 routes. The red-cx route has hostname http://red-cx-project-mgtheboss.apps.hackathon.rhmi.io, service red-cx, target port 8080-tcp, and no tls termination. The sso route has hostname, https://sso-project-mgtheboss.apps.hackathon.rhmi.io, service sso, no target port, and re-encrypt tls termination. 

To test the app, please open [red-cx-project-mgtheboss.apps.hackathon.rhmi.io](http://red-cx-project-mgtheboss.apps.hackathon.rhmi.io/) on a modern browser (chrome is recommended). You will be redirected to the login page. Please enter username, test-user-1 and password, password to log in. After successful login, you will be redirected to the app. We encourage you to read the concepts based on which the app has been built. When done, please enter the desired no. of customers and then the probability values and the probability of all customers having a good experience will be in front of you. 
