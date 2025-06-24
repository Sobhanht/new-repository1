# new-repository1
secound-repository
int ledState = LOW;  
unsigned long previousMillis = 0; 
unsigned long previousMillis01 = 0; 

const long interval = 1000;
const long interval01 = 3000;

const int ledPin = 10; 


void setup() {

  pinMode(ledPin, OUTPUT);

}

void loop() {
  // put your main code here, to run repeatedly:
  unsigned long currentMillis = millis();

  if (currentMillis - previousMillis >= interval) {
    previousMillis = currentMillis;
    if (ledState == LOW) {
      ledState = HIGH;
      } else {
      ledState = LOW;}
  }

  
    if (currentMillis - previousMillis01 >= interval01) {
    previousMillis01 = currentMillis;
    if (ledState == LOW) {
      ledState = HIGH;
    } else {
      ledState = LOW;
     }

 }
}
