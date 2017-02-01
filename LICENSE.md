//Muhammed Ali ÖZEN
const int led = 6; // Ledin hangi bacağa bağlandığını tanımladık
const int pirPin = 5; //Pır sensörünün hangi bacağa bağlandığını tanımladık
int pirDeger; 

void setup() {
pinMode(pirPin, INPUT); //pır sensörünü giriş olarak atadık
pinMode(led, OUTPUT); // ledimizi çıkış olarak atadık
}

void loop() {

pirDeger = digitalRead(pirPin);
if (pirDeger == HIGH) // hareket algılandığında
{
digitalWrite(led, HIGH); //led yansın
}
if (pirDeger == LOW) // hareket algılanmadığında
{
digitalWrite(led, LOW); //led sönsün 


}
}
