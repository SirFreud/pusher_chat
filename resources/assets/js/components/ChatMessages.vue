<template>
    <ul class="chat">
        <li v-for="message in messages" class="left clearfix">
            <div class="chat-body clearfix">
                <div class="header">
                    <strong class="primary-font">
                        {{ message.user.name }}
                    </strong>
                </div>
                <p>
                    {{ message.message }}
                </p>
            </div>
        </li>
            
        </li>
    </ul>
</template>

<script>
    export default {
        props: ['messages']
    };
</script>
