<template>
<nav class="main">
    <ul>
        <li><a href="/">Home</a></li>
        <li><a href="#">Link 1</a></li>
        <li><a href="#">Link 2</a></li>
        <li><a href="#">Link 3</a></li>
        <slot></slot>
    </ul>
</nav>
</template>
    
<style lang="scss">
nav.main {
    ul {
        margin: 0;
        padding: 0;
        list-style-type: none;
    }
    & > ul {
        display: flex;
    }
    a {
        color: inherit;
        text-decoration: none;
        padding: 0 1em;
        display: flex;
        align-items: center;
        justify-content: center;
        text-align: center;
        &:hover {
            background-color: hsl(var(--hue), var(--sat), 30%);
        }
    }
}
</style>

<script>
export default {
    
}
</script>