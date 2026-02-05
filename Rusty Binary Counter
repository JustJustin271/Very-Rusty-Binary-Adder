const int led1 = 10; //8's pin
const int led2 = 11; //4's pin
const int led3 = 12; //2's pin
const int led4 = 13; //1's pin

const int btn = 2; //Button

int number = 0; 

void setup() {
  pinMode(led1, OUTPUT);
  pinMode(led2, OUTPUT);
  pinMode(led3, OUTPUT);
  pinMode(led4, OUTPUT);
  pinMode(btn, INPUT_PULLUP);
}

void loop() {
  if (digitalRead(btn) == LOW) {
    if(number == 15){
      number = 0; 
    }
    number += 1;
  }

  //--Logic :) 

  digitalWrite(led4, ((number & 1) == 1) ? HIGH : LOW);

  digitalWrite(led3, ((number & 2) == 2) ? HIGH : LOW);

  digitalWrite(led2, ((number & 4) == 4) ? HIGH : LOW);

  digitalWrite(led1, ((number & 8) == 8) ? HIGH : LOW);

  delay(250); //Bouncy Bouncy
  
}
