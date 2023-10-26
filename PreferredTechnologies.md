## Prefered technologies

### Front end
ReactJS vs Angular

I would personally give advantage to React over Angular, especially because we might need very optimized rendering for hall presentation with seats.

If we go with React there is technology: https://reactnative.dev/ which is used to build Instagram. This should be good enough for us too. 

### Backend
Although Microservice architecture encouraging using different language for different services, we don't have reason for that. 
it's much easier to focus on one language/platform. 

#### Option 1.
If we have freedom to use whatever we want I would go with Python, especially because it's performing better than other popular language in some cloud environment use cases (i.e. Lambda functions.)

#### Option 2.
If we heavy depends on some Windows related feature, for which we cannot find api in other (Python) language, we would be forced to use .NET which is still great platofrm for web development. 

## Microservice communication 
For microservice communication and preserving logs and creating materialized views I believe Kafka could be the best solution in cooperation with https://www.confluent.io/ who offer Kafka as SAAS. By the way they are behind Kafka project, they build it.
Using a third party as SAAS, in this case could reduce costs, as we would need complex deployment and maintenance. 

## Storages
For internal storages we will use classic relation database like postgresql, and for the cases when we need speed, and scalability we will use DynamoDB (In user application services)

## Video Streaming
For the purpose of trailers, we have few options. 
- In house + cloud for deployment
  I found this expensive
- Using videos from IMDB  Could be a solid solution at least in the beginning to boost development. Not sure if this should be final one.
- Hosting videos on professional platforms like Vimeo (no commercials like on YouTube, etc...)  I would prefer this one.

... to be continued
