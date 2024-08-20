const int switchPin=4;
const int ledPin=13;
int switchState=0;
void setup(){
  pinMode(ledPin,OUTPUT);
  pinMode(switchPin,INPUT);
  
}
void loop() {
  switchState=digitalRead(switchPin);
  if(switchState==HIGH){
    digitalWrite(ledPin,HIGH);
    delay(1000);
  }
    digitalWrite(ledPin,LOW);
 
}
