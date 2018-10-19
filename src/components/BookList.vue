<template>
<div>
    <h1>{{title}}</h1>
    <ul>
        <book-item v-for="book in books" :book='book'></book-item>
    </ul>
</div>
    
</template>

<script>
import BookItem from './BookItem';
export default {
    name: 'BookList',
    components: {
        BookItem
    },
    data() {
        return {
            title: 'All Books',
            books: [
                {title: 'coding for idiots', author: 'An Idio'},
                {title: 'American Gods', author: 'An Idio'},
                {title: 'whos comment is it anyway?', author: 'weird al'},
            ]
        }
    }
}
</script>

<style>
h1, h2 {
    font-weight: normal;
}
ul {
list-style-type: none;
padding: 0;
}
li {
display: block;
margin: 0 10px;
}
</style>


