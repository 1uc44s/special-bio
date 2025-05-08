Site başlığını değiştirmek için alternatifler:

TypeWrite (default hali)

<script>
  const msg = "@1uc44s";
  let index = 0;
  let reverse = false;

  setInterval(() => {
    document.title = msg.substring(0, index);

    if (!reverse) {
      index++;
      if (index > msg.length) {
        reverse = true;
        setTimeout(() => {}, 1000);
      }
    } else {
      index--;
      if (index < 0) {
        reverse = false;
      }
    }
  }, 250);
</script>


Başlık yanında otomatik emoji değişiyor

<script>
  const emojis = ["🚀", "✨", "👾", "💻", "🎧", "🕶️"]; //emojileri değiştirebilirsiniz veya çoğalta bilirsiniz
  let i = 0;

  setInterval(() => {
    document.title = `@1uc44s ${emojis[i % emojis.length]}`;
    i++;
  }, 600);
</script>


Başlık yana doğru kayıyor

<script>
  const text = "@1uc44s - always money ";
  let i = 0;
  setInterval(() => {
    document.title = text.slice(i) + text.slice(0, i);
    i = (i + 1) % text.length;
  }, 200);
</script>



Kullanmak için sadece <script> yazılarının atasını kopyalayın ve index.html sayfasındaki <script> içini silip bunu yapıştırın.




Müzik ekleme konusu üzerinde çalışıyorum.