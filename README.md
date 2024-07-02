# Deaf-Driver-project               ARUDINO CODE

int mic=3;
int motor=8;
int led=9;
void setup() {
 pinMode(mic,INPUT);
 pinMode(motor,OUTPUT);
 pinMode(led,OUTPUT);
 Serial.begin(9600);
 // put your setup code here, to run once:
}
void loop() {
 Serial.println(digitalRead(mic));
 if(digitalRead (mic)==0)
 {
 digitalWrite(motor,HIGH);
 digitalWrite(led,HIGH);
 delay(3000);
 }
 else
 {
 digitalWrite(motor,LOW);
 digitalWrite(led,LOW);
 } // put your main code here, to run repeatedly:
}
