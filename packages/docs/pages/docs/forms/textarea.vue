<template lang="md" src="./textarea.md" />
<script>
import View from '@components/docs/View';
import { head } from "@helpers/head";
import { ITextarea } from "@inkline/inkline/src/components";

export default {
    extends: View,
    name: 'TextareaView',
    layout: 'documentation',
    head: head(),
    components: {
        ITextarea
    },
    data () {
        const sampleText = 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.';

        return {
            textareaValue: '',
            disabledTextareaValue: '',
            clearableTextareaValue: '',
            prefixTextareaValue: sampleText,
            suffixTextareaValue: sampleText,
            prefixSuffixTextareaValue: sampleText,
            prependTextareaValue: '',
            appendTextareaValue: '',
            prependAppendTextareaValue: '',
            smTextareaValue: '',
            mdTextareaValue: '',
            lgTextareaValue: '',
            labelDefaultTextareaValue: '',
            labelLeftTextareaValue: '',
            labelRightTextareaValue: ''
        };
    }
};
</script>
