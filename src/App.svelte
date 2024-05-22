<script>
  import logo from './assets/logo.svg';
  import Picture from './lib/Picture.svelte';
  import Note from './lib/Note.svelte';

  import imageA from './assets/IMG_0498.jpg';
  import imageB from './assets/20240223_183424.jpg';
  import imageC from './assets/Screenshot_20240401_074841_Samsung_Notes.jpg';
  import imageD from './assets/d.webp';

  function dday(d1, d2) {
        var t2 = d2.getTime();
        var t1 = d1.getTime();
 
        return Math.floor((t2-t1)/(24*3600*1000))+1;
  }
</script>

<h3 id=b>
  There's nothing that cannot made with the machine.<br/>
  기계로 만들 수 없는 것은 없다, 단지 시도하지 않을 뿐.
</h3>

<sidebar>
  <Picture img={imageA} deg={10}>소중한 추억</Picture>
  <Note color='#D3EFF3'>
    <p style="font-size: .9rem;">
      🎗️ Kwak<br/>
      We miss u. (D+{dday(new Date('Oct, 5, 2023'), new Date())})<br/>
      <br/>
      ❤️ with Java<br/>
      Since 2020 (D+{dday(new Date('Feb, 1, 2020'), new Date())})<br/>
      <br/>
      💙 with A320N<br/>
      Since 2021 (D+{dday(new Date('Jan, 7, 2021'), new Date())})<br/>
      <br/>
      🎉 with 1-5 at SRIHS<br/>
      Since 2024 (D+{dday(new Date('Mar, 3, 2024'), new Date())})
    </p>
  </Note>
  <Picture img={imageB} deg={-10}>대충 캠핑</Picture>
</sidebar>
<main>
  <h1>Yellowstrawberry</h1>
  <p>Student Engineer</p>
  <br/><br/>
  <h3>Available Languages</h3>
  <p>: Java, Typescript, Python, C/C++, C#, Rust, SQL, Swift, Dart, Javascript, Korean, English</p>
  <br/><br/>
  <h3>Available Skills</h3>
  <p>: Svelte, Quarkus, Springboot, Bukkit, Forge, Android, iOS, Embedded, Flutter, Unreal, Untiy</p>
  <br/><br/>
  <h3>Information</h3>
  <p>: SRIHS 119th (Software, AnA 15th)<br/>
    ROIN.GG Developer
  </p>
  <br/>
  <div id="cphead"></div>
  <div id="cpbody"><div id="logo"><img src={logo} alt="logo"/><h2>&nbsp;@Yellowstrawberrys <small>(Github)</small></h2></div><div id="floppy"></div></div>
</main>
<sidebar>
  <Picture img={imageC} deg={5}>SARD 만우절</Picture>
  <Picture img={imageD} deg={-7}>내 남친</Picture>
  <Note color='#F6EEA6' deg={2}>
    <p style="font-size: .9rem;">
      Instagram<br/>
      - @yellowstrawberry3009<br/>
      <br/>
      Github<br/>
      - @yellowstrawberrys<br/>
      - @yellowstrawberry<br/>
      <br/>
      Youtube<br/>
      - @yellowstrawberry
    </p>
  </Note>
</sidebar>