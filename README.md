# shortcircuitint;
int redLED = 11;
int yellowLED = 10;
int greenLED = 9;
int button = 2;

void setup() {
  pinMode(redLED, OUTPUT);
  pinMode(yellowLED, OUTPUT);
  pinMode(greenLED, OUTPUT);
  pinMode(button, INPUT);
}

void loop() {
  if (digitalRead(button) == HIGH) {
 
    digitalWrite(redLED, HIGH);
    digitalWrite(yellowLED, LOW);
    digitalWrite(greenLED, LOW);
    delay(5000); 
  } 
   else 
        {
 
    digitalWrite(greenLED, HIGH);
     digitalWrite(yellowLED, LOW);
    digitalWrite(redLED, LOW);
    delay(1000); 
      if (digitalRead(button) == HIGH) {
 
    digitalWrite(redLED, HIGH);
    digitalWrite(yellowLED, LOW);
    digitalWrite(greenLED, LOW);
        delay(5000); }
    
   
    digitalWrite(yellowLED, HIGH);
     digitalWrite(greenLED, LOW);
       digitalWrite(redLED, LOW);
    delay(2000); 
         if (digitalRead(button) == HIGH) {
 
    digitalWrite(redLED, HIGH);
    digitalWrite(yellowLED, LOW);
    digitalWrite(greenLED, LOW);
           delay(2000); }
    
    
    digitalWrite(redLED, HIGH);
     digitalWrite(yellowLED, LOW);
     digitalWrite(greenLED, LOW);
    delay(3000); 
            if (digitalRead(button) == HIGH) {
 
    digitalWrite(redLED, HIGH);
    digitalWrite(yellowLED, LOW);
    digitalWrite(greenLED, LOW);
              delay(1000); }
    
    
  }
}
