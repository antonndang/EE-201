# Arduino
## Exercise I & II
```
void setup() {
  // put your setup code here, to run once:
  pinMode(13, OUTPUT);

}

void loop() {
  // put your main code here, to run repeatedly:
  digitalWrite(13, HIGH);
  delay(1000);
  digitalWrite(13, LOW);
  delay(1000);

}
```
### Exercise III

```
void setup() {
  // put your setup code here, to run once:
//pinMode(13, OUTPUT);
Serial.begin(9600);
pinMode(7, INPUT);
}

void loop() {
  // put your main code here, to run repeatedly:
  // digitalWrite(13, HIGH);
  // delay(1000);
  // digitalWrite(13, LOW);
  // delay(1000);
if(digitalRead(7)){
  Serial.println("Hello World!");
}
else{
  Serial.println("It's 2023");
}
}
```

#### Exercise IV (test the 7 Segment)

```
// void setup() {
// put your setup code here, to run once:
// pinMode(8, OUTPUT);
// pinMode(2, OUTPUT);
// pinMode(3, OUTPUT);
// pinMode(4, OUTPUT);
// pinMode(5, OUTPUT);
// pinMode(6, OUTPUT);
// pinMode(7, OUTPUT);


// }

// void loop() {
//   // put your main code here, to run repeatedly:
//   // digitalWrite(8, HIGH);

//   // digitalWrite(2, HIGH);
//   // digitalWrite(3, HIGH);
//   // digitalWrite(4, HIGH);
//   // digitalWrite(5, HIGH);
//   // digitalWrite(6, HIGH);
//   // digitalWrite(7, HIGH);
//   // delay(1500);
//   // digitalWrite(8, LOW);
//   // digitalWrite(2, LOW);
//   // digitalWrite(3, LOW);
//   // digitalWrite(4, LOW);
//   // digitalWrite(5, LOW);
//   // digitalWrite(6, LOW);
//   // digitalWrite(7, LOW);


//   // delay(1500);
 

// }

```


##### Exercise IV (Display 9-0 every 1.5 second per numbers)

```
int pinA = 8;
int pinB = 7;
int pinC = 6;
int pinD = 5;
int pinE = 4;
int pinF = 3;
int pinG = 2;


void setup() {
  // put your setup code here, to run once:
  pinMode(pinA, OUTPUT);
  pinMode(pinB, OUTPUT);
  pinMode(pinC, OUTPUT);
  pinMode(pinD, OUTPUT);
  pinMode(pinE, OUTPUT);
  pinMode(pinF, OUTPUT);
  pinMode(pinG, OUTPUT);
}

void loop() {
  // put your main code here, to run repeatedly:

  // #9
  digitalWrite(pinA , 0);
  digitalWrite(pinB , 0);
  digitalWrite(pinC , 0);
  digitalWrite(pinD , 0);
  digitalWrite(pinE , 1);
  digitalWrite(pinF , 0);
  digitalWrite(pinG , 0);
  delay(1500);

  // #8
  digitalWrite(pinA , 0);
  digitalWrite(pinB , 0);
  digitalWrite(pinC , 0);
  digitalWrite(pinD , 0);
  digitalWrite(pinE , 0);
  digitalWrite(pinF , 0);
  digitalWrite(pinG , 0);
  delay(1500);

  // #7
  digitalWrite(pinA , 0);
  digitalWrite(pinB , 0);
  digitalWrite(pinC , 0);
  digitalWrite(pinD , 1);
  digitalWrite(pinE , 1);
  digitalWrite(pinF , 1);
  digitalWrite(pinG , 1);
  delay(1500);

    // #6
  digitalWrite(pinA , 0);
  digitalWrite(pinB , 1);
  digitalWrite(pinC , 0);
  digitalWrite(pinD , 0);
  digitalWrite(pinE , 0);
  digitalWrite(pinF , 0);
  digitalWrite(pinG , 0);
  delay(1500);

  // #5
  digitalWrite(pinA , 0);
  digitalWrite(pinB , 1);
  digitalWrite(pinC , 0);
  digitalWrite(pinD , 0);
  digitalWrite(pinE , 1);
  digitalWrite(pinF , 0);
  digitalWrite(pinG , 0);
  delay(1500);

  // #4
  digitalWrite(pinA , 1);
  digitalWrite(pinB , 0);
  digitalWrite(pinC , 0);
  digitalWrite(pinD , 1);
  digitalWrite(pinE , 1);
  digitalWrite(pinF , 0);
  digitalWrite(pinG , 0);
  delay(1500);

  // #3
  digitalWrite(pinA , 0);
  digitalWrite(pinB , 0);
  digitalWrite(pinC , 0);
  digitalWrite(pinD , 0);
  digitalWrite(pinE , 1);
  digitalWrite(pinF , 1);
  digitalWrite(pinG , 0);
  delay(1500);

  // #2
  digitalWrite(pinA , 0);
  digitalWrite(pinB , 0);
  digitalWrite(pinC , 1);
  digitalWrite(pinD , 0);
  digitalWrite(pinE , 0);
  digitalWrite(pinF , 1);
  digitalWrite(pinG , 0);
  delay(1500);

  // #1
  digitalWrite(pinA , 1);
  digitalWrite(pinB , 0);
  digitalWrite(pinC , 0);
  digitalWrite(pinD , 1);
  digitalWrite(pinE , 1);
  digitalWrite(pinF , 1);
  digitalWrite(pinG , 1);
  delay(1500);

  // #0
  digitalWrite(pinA , 0);
  digitalWrite(pinB , 0);
  digitalWrite(pinC , 0);
  digitalWrite(pinD , 0);
  digitalWrite(pinE , 0);
  digitalWrite(pinF , 0);
  digitalWrite(pinG , 1);
  delay(1500);


}
```
