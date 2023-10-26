## Analiza rizika

### Tačke integracije su glavni rizici po stabilnost sistema i moraju biti dizajnirane na odgovarajući način.

Dve osnovne tačke integracije su prema 
- Payment procesorima (na primer Stripe), na šta često ne možemo da utičemo, međutim možemo u sradnji sa njima da izaberemo preferibilni načnin komunikacije (verovatno asihorni). Takođe treba razmotriti da imamo i backup payment procesor.
- Integracija sa servisom za hranu i piće. Ovo nije toliko kritično i ako je deo našeg pod-sistema možemo dosta da utičemo na stabilnost i skalabilnost po potrebi.
- Integracija sa Kafka SAAS provider-m Confluent Cloud. Confulend Cloud je prilično

### Dostupnost

Rizik dostupnosti platforme najbolje je rešiti tako što bi podigli dva okruženja (dva VPC-ja verovatno) u dve različite geografske zone sa load balancer-om i Fargate-om (ili nekom drugom tehnologijom za kontejnere)



