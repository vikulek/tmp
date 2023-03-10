# Практическая работа №1
## Выполнила Турбина В.А., БИСО-03-20

```
@startuml
left to right direction
skinparam packageStyle rect
actor client
actor bank
rectangle ATM {
  client-- (check cash)
  client-- (withdraw cash)
  client-- (put money on the card)
  (withdraw cash) <- (check cash) : extends
  bank -- (check rest)
}
@enduml
```
