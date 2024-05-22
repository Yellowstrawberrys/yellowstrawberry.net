<script>
    export let color;
    export let deg = 0;

    const style = {
        'background-color': color,
        'transform': 'translate(-50%) rotate('+deg+'deg)'
    }

    /**
     * @param {{ [x: string]: any; }} obj
     */
    function cssStringify(obj) {
        return Object.keys(obj).map(k => `${k}: ${obj[k]}`).join(';')
    }
</script>

<div id=note style={cssStringify(style)}>
<slot></slot>
</div>

<style>
    #note {
        width: 16rem;
        padding: .6rem;
        box-shadow: 0 0 .2rem rgba(0,0,0, .25);
        margin-left: 50%;
    }
</style>