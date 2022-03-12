# Hava-Sicakligina-Gore-Etkinlik-Onerme
Patika.dev > Java101 > Koşullu İfadeler ve Kod Blokları > Pratik4 - Hava Sıcaklığına Göre Etkinlik Önerme

## Koşullar
- Sıcaklık 5'dan küçük ise "Kayak" yapmayı öner.
- Sıcaklık 5 ve 15 arasında ise "Sinema" etkinliğini öner.
- Sıcaklık 15 ve 25 arasında ise "Piknik" etkinliğini öner.
- Sıcaklık 25'ten büyük ise "Yüzme" etkinliğini öner.
### Aynı örnek üzerinden if koşulları başka hangi şekilde oluşturulabilirdi farklı çözüm yolları bulunuz.

        import java.util.*;

        public class havaSicakliginaGoreEtkinlikOnerme {
        
            public static void main(String[] args) {
        
                // Yeni bir tarayıcı(scanner) oluştur.
                Scanner sc= new Scanner(System.in);
                
                // Kullanıcıdan sıcaklık değerlerini al.
                System.out.println("Sıcaklık giriniz: ");
                int heat = sc.nextInt();
                
                if(heat <= 25) {
                    if(heat > 15 && heat <= 25) 
                        System.out.println("Pikniğe gidebilirsiniz.");
            
                    else if(heat >= 5 && heat <= 15)
                        System.out.println("Sinemaya gidebilirsiniz.");

                    else
                        System.out.println("Kayak yapabilirsiniz.");
                }

                else {
                    System.out.println("Yüzmeye gidebilirsiniz.");
                }
            }
        }
