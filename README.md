# cds
this code used **cds**

## parts list

* arduino
* cds
* wire
* register
* breadboard


## arduino

```cpp
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  pinMode(5,OUTPUT);
  digitalWrite(5,HIGH);
  
}

void loop() {
  // put your main code here, to run repeatedly:
 
  int value;
  value=analogRead(A0);
  Serial.println(value);
 
  delay(200);
  
  if(value<400) {
  digitalWrite(5,LOW);
  }else{
  digitalWrite(5,HIGH);

  } 
  }
  
  ```
  ![arduino cds](https://github.com/sunny9645/cds/blob/master/cds_bb.jpg)
