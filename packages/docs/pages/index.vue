<template src="./index.html" />
<style lang="scss" src="./index.scss"></style>
<script>
import {
    IHeader,
    IContainer,
    IRow,
    IColumn,
    IButton,
    ICard,
    ITooltip
} from "@inkline/inkline/src/index";
import { head } from '@helpers/head'
import Sponsor from '@components/Sponsor';
import GithubButton from 'vue-github-button'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';

export default {
    name: 'IndexView',
    layout: 'Default',
    head: head({
        preserve: {
            description: true
        }
    }),
    components: {
        IHeader,
        IContainer,
        IRow,
        IColumn,
        IButton,
        ICard,
        ITooltip,
        GithubButton,
        Sponsor,
        FontAwesomeIcon
    },
    data() {
        const defaultSponsor = {
            title: 'Become a sponsor',
            url: 'https://www.patreon.com/bePatron?u=18449490',
            placeholder: true
        };

        return {
            sponsors: {
                large: [
                    defaultSponsor,
                    defaultSponsor,
                    {
                        title: 'Inkline - Vue.js UI/UX Library',
                        image: require('@/static/images/sponsors/large/inkline.png'),
                        url: 'https://inkline.io',
                        default: true
                    },
                    defaultSponsor,
                    defaultSponsor
                ]
            }
        };
    }
};
</script>
