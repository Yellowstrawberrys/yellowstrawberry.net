<script>
  export let img;
  export let deg = 0;

  const style = {
      'width': '95%',
      'height': '100%',
      'background-size': 'cover',
      'background-position': 'center',
      'background-image': 'url('+img+')',
  }

  const pic = {
    'transform': 'translate(-50%) rotate('+deg+'deg)'
  }

  /**
   * @param {{ [x: string]: any; }} obj
   */
  function cssStringify(obj) {
      return Object.keys(obj).map(k => `${k}: ${obj[k]}`).join(';')
  }
</script>

<div class="pic" style={cssStringify(pic)}>
  <div id="image" style={cssStringify(style)}></div>
  <p><slot></slot></p>
</div>

<style>
  .pic {
    margin-left: 50%;
    display: grid;
    justify-items: center;
    padding: .6rem;
    width: 13rem;
    height: 17rem;
    grid-template-rows: 80% 20%;
    background-color: #F9F6EF;
    box-shadow: 0 0 .2rem rgba(0,0,0, .25);
  }
</style>