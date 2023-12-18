
# CKEditor 5 Custom




## Installation

Install my-project with npm

```bash
    npm i @ckeditor-super/ckeditor5-super-custom
  
    <script setup>
    import Editor from '@ckeditor-super/ckeditor5-super-custom'

    const editor = Editor
    </script>
    <template>
    <div class="w-full">
        <ClientOnly>
        <CkeditorNuxt
            :editor="editor"
        />
        </ClientOnly>
    </div>
    </template>
    
    <style lang="scss">
    .ck-editor {
    p {
        display: block;
        -webkit-margin-before: 1__qem;
        -webkit-margin-after: 1__qem;
        -webkit-margin-start: 0;
        -webkit-margin-end: 0;
    }

    div {
        display: block;
    }

    layer {
        display: block;
    }

    article,
    aside,
    footer,
    header,
    hgroup,
    main,
    nav,
    section {
        display: block;
    }

    marquee {
        display: inline-block;
    }

    address {
        display: block;
    }

    blockquote {
        display: block;
        -webkit-margin-before: 1__qem;
        -webkit-margin-after: 1em;
        -webkit-margin-start: 40px;
        -webkit-margin-end: 40px;
    }

    figcaption {
        display: block;
    }

    figure {
        display: block;
        -webkit-margin-before: 1em;
        -webkit-margin-after: 1em;
        -webkit-margin-start: 40px;
        -webkit-margin-end: 40px;
    }

    q {
        display: inline;
    }

    q:before {
        content: open-quote;
    }

    q:after {
        content: close-quote;
    }

    center {
        display: block;
        /* special centering to be able to emulate the html4/netscape behaviour */
        text-align: -webkit-center;
    }

    hr {
        display: block;
        -webkit-margin-before: 0.5em;
        -webkit-margin-after: 0.5em;
        -webkit-margin-start: auto;
        -webkit-margin-end: auto;
        border-style: inset;
        border-width: 1px;
    }

    map {
        display: inline;
    }

    video {
        object-fit: contain;
    }

    /* heading elements */
    h1 {
        display: block;
        font-size: 2em;
        -webkit-margin-before: 0.67__qem;
        -webkit-margin-after: 0.67em;
        -webkit-margin-start: 0;
        -webkit-margin-end: 0;
        font-weight: bold;
    }

    :-webkit-any(article, aside, nav, section) h1 {
        font-size: 1.5em;
        -webkit-margin-before: 0.83__qem;
        -webkit-margin-after: 0.83em;
    }

    :-webkit-any(article, aside, nav, section) :-webkit-any(article, aside, nav, section) h1 {
        font-size: 1.17em;
        -webkit-margin-before: 1__qem;
        -webkit-margin-after: 1em;
    }

    :-webkit-any(article, aside, nav, section) :-webkit-any(article, aside, nav, section) :-webkit-any(article, aside, nav, section) h1 {
        font-size: 1em;
        -webkit-margin-before: 1.33__qem;
        -webkit-margin-after: 1.33em;
    }

    :-webkit-any(article, aside, nav, section) :-webkit-any(article, aside, nav, section) :-webkit-any(article, aside, nav, section) :-webkit-any(article, aside, nav, section) h1 {
        font-size: 0.83em;
        -webkit-margin-before: 1.67__qem;
        -webkit-margin-after: 1.67em;
    }

    :-webkit-any(article, aside, nav, section) :-webkit-any(article, aside, nav, section) :-webkit-any(article, aside, nav, section) :-webkit-any(article, aside, nav, section) :-webkit-any(article, aside, nav, section) h1 {
        font-size: 0.67em;
        -webkit-margin-before: 2.33__qem;
        -webkit-margin-after: 2.33em;
    }

    h2 {
        display: block;
        font-size: 1.5em;
        -webkit-margin-before: 0.83__qem;
        -webkit-margin-after: 0.83em;
        -webkit-margin-start: 0;
        -webkit-margin-end: 0;
        font-weight: bold;
    }

    h3 {
        display: block;
        font-size: 1.17em;
        -webkit-margin-before: 1__qem;
        -webkit-margin-after: 1em;
        -webkit-margin-start: 0;
        -webkit-margin-end: 0;
        font-weight: bold;
    }

    h4 {
        display: block;
        -webkit-margin-before: 1.33__qem;
        -webkit-margin-after: 1.33em;
        -webkit-margin-start: 0;
        -webkit-margin-end: 0;
        font-weight: bold;
    }

    h5 {
        display: block;
        font-size: 0.83em;
        -webkit-margin-before: 1.67__qem;
        -webkit-margin-after: 1.67em;
        -webkit-margin-start: 0;
        -webkit-margin-end: 0;
        font-weight: bold;
    }

    h6 {
        display: block;
        font-size: 0.67em;
        -webkit-margin-before: 2.33__qem;
        -webkit-margin-after: 2.33em;
        -webkit-margin-start: 0;
        -webkit-margin-end: 0;
        font-weight: bold;
    }

    /* tables */
    table {
        display: table;
        border-collapse: separate;
        border-spacing: 2px;
        border-color: gray;
    }

    thead {
        display: table-header-group;
        vertical-align: middle;
        border-color: inherit;
    }

    tbody {
        display: table-row-group;
        vertical-align: middle;
        border-color: inherit;
    }

    tfoot {
        display: table-footer-group;
        vertical-align: middle;
        border-color: inherit;
    }

    /* for tables without table section elements (can happen with XHTML or dynamically created tables) */
    table>tr {
        vertical-align: middle;
    }

    col {
        display: table-column;
    }

    colgroup {
        display: table-column-group;
    }

    tr {
        display: table-row;
        vertical-align: inherit;
        border-color: inherit;
    }

    td,
    th {
        display: table-cell;
        vertical-align: inherit;
    }

    th {
        font-weight: bold;
    }

    caption {
        display: table-caption;
        text-align: -webkit-center;
    }

    /* lists */
    ul,
    menu,
    dir {
        display: block;
        list-style-type: disc;
        -webkit-margin-before: 1__qem;
        -webkit-margin-after: 1em;
        -webkit-margin-start: 0;
        -webkit-margin-end: 0;
        -webkit-padding-start: 40px;
    }

    ol {
        display: block;
        list-style-type: decimal;
        -webkit-margin-before: 1__qem;
        -webkit-margin-after: 1em;
        -webkit-margin-start: 0;
        -webkit-margin-end: 0;
        -webkit-padding-start: 40px;
    }

    li {
        display: list-item;
        text-align: -webkit-match-parent;
    }

    ul ul,
    ol ul {
        list-style-type: circle;
    }

    ol ol ul,
    ol ul ul,
    ul ol ul,
    ul ul ul {
        list-style-type: square;
    }

    dd {
        display: block;
        -webkit-margin-start: 40px;
    }

    dl {
        display: block;
        -webkit-margin-before: 1__qem;
        -webkit-margin-after: 1em;
        -webkit-margin-start: 0;
        -webkit-margin-end: 0;
    }

    dt {
        display: block;
    }

    ol ul,
    ul ol,
    ul ul,
    ol ol {
        -webkit-margin-before: 0;
        -webkit-margin-after: 0;
    }

    /* form elements */
    form {
        display: block;
        margin-top: 0__qem;
    }

    label {
        cursor: default;
    }

    legend {
        display: block;
        -webkit-padding-start: 2px;
        -webkit-padding-end: 2px;
        border: none;
    }

    fieldset {
        display: block;
        -webkit-margin-start: 2px;
        -webkit-margin-end: 2px;
        -webkit-padding-before: 0.35em;
        -webkit-padding-start: 0.75em;
        -webkit-padding-end: 0.75em;
        -webkit-padding-after: 0.625em;
        border: 2px groove ThreeDFace;
        min-width: -webkit-min-content;
    }

    button {
        -webkit-appearance: button;
    }

    /* Form controls don't go vertical. */
    input,
    textarea,
    keygen,
    select,
    button,
    meter,
    progress {
        -webkit-writing-mode: horizontal-tb !important;
    }

    input,
    textarea,
    keygen,
    select,
    button {
        margin: 0__qem;
        font: -webkit-small-control;
        text-rendering: auto;
        /* FIXME: Remove when tabs work with optimizeLegibility. */
        color: initial;
        letter-spacing: normal;
        word-spacing: normal;
        line-height: normal;
        text-transform: none;
        text-indent: 0;
        text-shadow: none;
        display: inline-block;
        text-align: start;
    }

    input[type='hidden' i] {
        display: none;
    }

    input {
        -webkit-appearance: textfield;
        padding: 1px;
        background-color: white;
        border: 2px inset;
        -webkit-rtl-ordering: logical;
        -webkit-user-select: text;
        cursor: auto;
    }

    input[type='search' i] {
        -webkit-appearance: searchfield;
        box-sizing: border-box;
    }

    input::-webkit-textfield-decoration-container {
        display: flex;
        align-items: center;
        -webkit-user-modify: read-only !important;
        content: none !important;
    }

    input[type='search' i]::-webkit-textfield-decoration-container {
        direction: ltr;
    }

    input::-webkit-clear-button {
        -webkit-appearance: searchfield-cancel-button;
        display: inline-block;
        flex: none;
        -webkit-user-modify: read-only !important;
        -webkit-margin-start: 2px;
        opacity: 0;
        pointer-events: none;
    }

    input:enabled:read-write:-webkit-any(:focus, :hover)::-webkit-clear-button {
        opacity: 1;
        pointer-events: auto;
    }

    input[type='search' i]::-webkit-search-cancel-button {
        -webkit-appearance: searchfield-cancel-button;
        display: block;
        flex: none;
        -webkit-user-modify: read-only !important;
        -webkit-margin-start: 1px;
        opacity: 0;
        pointer-events: none;
    }

    input[type='search' i]:enabled:read-write:-webkit-any( :focus,
        :hover)::-webkit-search-cancel-button {
        opacity: 1;
        pointer-events: auto;
    }

    input[type='search' i]::-webkit-search-decoration {
        -webkit-appearance: searchfield-decoration;
        display: block;
        flex: none;
        -webkit-user-modify: read-only !important;
        -webkit-align-self: flex-start;
        margin: auto 0;
    }

    input[type='search' i]::-webkit-search-results-decoration {
        -webkit-appearance: searchfield-results-decoration;
        display: block;
        flex: none;
        -webkit-user-modify: read-only !important;
        -webkit-align-self: flex-start;
        margin: auto 0;
    }

    input::-webkit-inner-spin-button {
        -webkit-appearance: inner-spin-button;
        display: inline-block;
        cursor: default;
        flex: none;
        align-self: stretch;
        -webkit-user-select: none;
        -webkit-user-modify: read-only !important;
        opacity: 0;
        pointer-events: none;
    }

    input:enabled:read-write:-webkit-any( :focus,
        :hover)::-webkit-inner-spin-button {
        opacity: 1;
        pointer-events: auto;
    }

    keygen,
    select {
        border-radius: 5px;
    }

    keygen::-webkit-keygen-select {
        margin: 0px;
    }

    textarea {
        -webkit-appearance: textarea;
        background-color: white;
        border: 1px solid;
        -webkit-rtl-ordering: logical;
        -webkit-user-select: text;
        flex-direction: column;
        resize: auto;
        cursor: auto;
        padding: 2px;
        white-space: pre-wrap;
        word-wrap: break-word;
    }

    ::-webkit-input-placeholder {
        -webkit-text-security: none;
        color: darkGray;
        pointer-events: none !important;
    }

    input::-webkit-input-placeholder {
        white-space: pre;
        word-wrap: normal;
        overflow: hidden;
        -webkit-user-modify: read-only !important;
    }

    input[type='password' i] {
        -webkit-text-security: disc !important;
    }

    input[type='hidden' i],
    input[type='image' i],
    input[type='file' i] {
        -webkit-appearance: initial;
        padding: initial;
        background-color: initial;
        border: initial;
    }

    input[type='file' i] {
        align-items: baseline;
        color: inherit;
        text-align: start !important;
    }

    input:-webkit-autofill,
    textarea:-webkit-autofill,
    select:-webkit-autofill {
        background-color: #faffbd !important;
        background-image: none !important;
        color: #000000 !important;
    }

    input[type='radio' i],
    input[type='checkbox' i] {
        margin: 3px 0.5ex;
        padding: initial;
        background-color: initial;
        border: initial;
    }

    input[type='button' i],
    input[type='submit' i],
    input[type='reset' i] {
        -webkit-appearance: push-button;
        -webkit-user-select: none;
        white-space: pre;
    }

    input[type='file' i]::-webkit-file-upload-button {
        -webkit-appearance: push-button;
        -webkit-user-modify: read-only !important;
        white-space: nowrap;
        margin: 0;
        font-size: inherit;
    }

    input[type='button' i],
    input[type='submit' i],
    input[type='reset' i],
    input[type='file' i]::-webkit-file-upload-button,
    button {
        align-items: flex-start;
        text-align: center;
        cursor: default;
        color: ButtonText;
        padding: 2px 6px 3px 6px;
        border: 2px outset ButtonFace;
        background-color: ButtonFace;
        box-sizing: border-box;
    }

    input[type='range' i] {
        -webkit-appearance: slider-horizontal;
        padding: initial;
        border: initial;
        margin: 2px;
        color: #909090;
    }

    input[type='range' i]::-webkit-slider-container,
    input[type='range' i]::-webkit-media-slider-container {
        flex: 1;
        min-width: 0;
        box-sizing: border-box;
        -webkit-user-modify: read-only !important;
        display: flex;
    }

    input[type='range' i]::-webkit-slider-runnable-track {
        flex: 1;
        min-width: 0;
        -webkit-align-self: center;
        box-sizing: border-box;
        -webkit-user-modify: read-only !important;
        display: block;
    }

    input[type='range' i]::-webkit-slider-thumb,
    input[type='range' i]::-webkit-media-slider-thumb {
        -webkit-appearance: sliderthumb-horizontal;
        box-sizing: border-box;
        -webkit-user-modify: read-only !important;
        display: block;
    }

    input[type='button' i]:disabled,
    input[type='submit' i]:disabled,
    input[type='reset' i]:disabled,
    input[type='file' i]:disabled::-webkit-file-upload-button,
    button:disabled,
    select:disabled,
    keygen:disabled,
    optgroup:disabled,
    option:disabled,
    select[disabled]>option {
        color: GrayText;
    }

    input[type='button' i]:active,
    input[type='submit' i]:active,
    input[type='reset' i]:active,
    input[type='file' i]:active::-webkit-file-upload-button,
    button:active {
        border-style: inset;
    }

    input[type='button' i]:active:disabled,
    input[type='submit' i]:active:disabled,
    input[type='reset' i]:active:disabled,
    input[type='file' i]:active:disabled::-webkit-file-upload-button,
    button:active:disabled {
        border-style: outset;
    }

    option:-internal-spatial-navigation-focus {
        outline: black dashed 1px;
        outline-offset: -1px;
    }

    datalist {
        display: none;
    }

    area {
        display: inline;
        cursor: pointer;
    }

    param {
        display: none;
    }

    input[type='checkbox' i] {
        -webkit-appearance: checkbox;
        box-sizing: border-box;
    }

    input[type='radio' i] {
        -webkit-appearance: radio;
        box-sizing: border-box;
    }

    input[type='color' i] {
        -webkit-appearance: square-button;
        width: 44px;
        height: 23px;
        background-color: ButtonFace;
        /* Same as native_theme_base. */
        border: 1px #a9a9a9 solid;
        padding: 1px 2px;
    }

    input[type='color' i]::-webkit-color-swatch-wrapper {
        display: flex;
        padding: 4px 2px;
        box-sizing: border-box;
        -webkit-user-modify: read-only !important;
        width: 100%;
        height: 100%;
    }

    input[type='color' i]::-webkit-color-swatch {
        background-color: #000000;
        border: 1px solid #777777;
        flex: 1;
        min-width: 0;
        -webkit-user-modify: read-only !important;
    }

    input[type='color' i][list] {
        -webkit-appearance: menulist;
        width: 88px;
        height: 23px;
    }

    input[type='color' i][list]::-webkit-color-swatch-wrapper {
        padding-left: 8px;
        padding-right: 24px;
    }

    input[type='color' i][list]::-webkit-color-swatch {
        border-color: #000000;
    }

    input::-webkit-calendar-picker-indicator {
        display: inline-block;
        width: 0.66em;
        height: 0.66em;
        padding: 0.17em 0.34em;
        -webkit-user-modify: read-only !important;
        opacity: 0;
        pointer-events: none;
    }

    input::-webkit-calendar-picker-indicator:hover {
        background-color: #eee;
    }

    input:enabled:read-write:-webkit-any( :focus,
        :hover)::-webkit-calendar-picker-indicator,
    input::-webkit-calendar-picker-indicator:focus {
        opacity: 1;
        pointer-events: auto;
    }

    input[type='date' i]:disabled::-webkit-clear-button,
    input[type='date' i]:disabled::-webkit-inner-spin-button,
    input[type='datetime-local' i]:disabled::-webkit-clear-button,
    input[type='datetime-local' i]:disabled::-webkit-inner-spin-button,
    input[type='month' i]:disabled::-webkit-clear-button,
    input[type='month' i]:disabled::-webkit-inner-spin-button,
    input[type='week' i]:disabled::-webkit-clear-button,
    input[type='week' i]:disabled::-webkit-inner-spin-button,
    input:disabled::-webkit-calendar-picker-indicator,
    input[type='date' i][readonly]::-webkit-clear-button,
    input[type='date' i][readonly]::-webkit-inner-spin-button,
    input[type='datetime-local' i][readonly]::-webkit-clear-button,
    input[type='datetime-local' i][readonly]::-webkit-inner-spin-button,
    input[type='month' i][readonly]::-webkit-clear-button,
    input[type='month' i][readonly]::-webkit-inner-spin-button,
    input[type='week' i][readonly]::-webkit-clear-button,
    input[type='week' i][readonly]::-webkit-inner-spin-button,
    input[readonly]::-webkit-calendar-picker-indicator {
        visibility: hidden;
    }

    select {
        -webkit-appearance: menulist;
        box-sizing: border-box;
        align-items: center;
        border: 1px solid;
        white-space: pre;
        -webkit-rtl-ordering: logical;
        color: black;
        background-color: white;
        cursor: default;
    }

    select:not(:-internal-list-box) {
        overflow: visible !important;
    }

    select:-internal-list-box {
        -webkit-appearance: listbox;
        align-items: flex-start;
        border: 1px inset gray;
        border-radius: initial;
        overflow-x: hidden;
        overflow-y: scroll;
        vertical-align: text-bottom;
        -webkit-user-select: none;
        white-space: nowrap;
    }

    optgroup {
        font-weight: bolder;
        display: block;
    }

    option {
        font-weight: normal;
        display: block;
        padding: 0 2px 1px 2px;
        white-space: pre;
        min-height: 1.2em;
    }

    select:-internal-list-box optgroup option:before {
        content: '\00a0\00a0\00a0\00a0';
    }

    select:-internal-list-box option,
    select:-internal-list-box optgroup {
        line-height: initial !important;
    }

    select:-internal-list-box:focus option:checked {
        background-color: -internal-active-list-box-selection !important;
        color: -internal-active-list-box-selection-text !important;
    }

    select:-internal-list-box option:checked {
        background-color: -internal-inactive-list-box-selection !important;
        color: -internal-inactive-list-box-selection-text !important;
    }

    select:-internal-list-box:disabled option:checked,
    select:-internal-list-box option:checked:disabled {
        color: gray !important;
    }

    select:-internal-list-box hr {
        border-style: none;
    }

    output {
        display: inline;
    }

    /* meter */
    meter {
        -webkit-appearance: meter;
        box-sizing: border-box;
        display: inline-block;
        height: 1em;
        width: 5em;
        vertical-align: -0.2em;
    }

    meter::-webkit-meter-inner-element {
        -webkit-appearance: inherit;
        box-sizing: inherit;
        -webkit-user-modify: read-only !important;
        height: 100%;
        width: 100%;
    }

    meter::-webkit-meter-bar {
        background: linear-gradient(to bottom,
            #ddd,
            #eee 20%,
            #ccc 45%,
            #ccc 55%,
            #ddd);
        height: 100%;
        width: 100%;
        -webkit-user-modify: read-only !important;
        box-sizing: border-box;
    }

    meter::-webkit-meter-optimum-value {
        background: linear-gradient(to bottom,
            #ad7,
            #cea 20%,
            #7a3 45%,
            #7a3 55%,
            #ad7);
        height: 100%;
        -webkit-user-modify: read-only !important;
        box-sizing: border-box;
    }

    meter::-webkit-meter-suboptimum-value {
        background: linear-gradient(to bottom,
            #fe7,
            #ffc 20%,
            #db3 45%,
            #db3 55%,
            #fe7);
        height: 100%;
        -webkit-user-modify: read-only !important;
        box-sizing: border-box;
    }

    meter::-webkit-meter-even-less-good-value {
        background: linear-gradient(to bottom,
            #f77,
            #fcc 20%,
            #d44 45%,
            #d44 55%,
            #f77);
        height: 100%;
        -webkit-user-modify: read-only !important;
        box-sizing: border-box;
    }

    /* progress */
    progress {
        -webkit-appearance: progress-bar;
        box-sizing: border-box;
        display: inline-block;
        height: 1em;
        width: 10em;
        vertical-align: -0.2em;
    }

    progress::-webkit-progress-inner-element {
        -webkit-appearance: inherit;
        box-sizing: inherit;
        -webkit-user-modify: read-only;
        height: 100%;
        width: 100%;
    }

    progress::-webkit-progress-bar {
        background-color: gray;
        height: 100%;
        width: 100%;
        -webkit-user-modify: read-only !important;
        box-sizing: border-box;
    }

    progress::-webkit-progress-value {
        background-color: green;
        height: 100%;
        width: 50%;
        /* should be removed later */
        -webkit-user-modify: read-only !important;
        box-sizing: border-box;
    }

    /* inline elements */
    u,
    ins {
        text-decoration: underline;
    }

    strong,
    b {
        font-weight: bold;
    }

    i,
    cite,
    em,
    var,
    address,
    dfn {
        font-style: italic;
    }

    tt,
    code,
    kbd,
    samp {
        font-family: monospace;
    }

    pre,
    xmp,
    plaintext,
    listing {
        display: block;
        font-family: monospace;
        white-space: pre;
        margin: 1__qem 0;
    }

    mark {
        background-color: yellow;
        color: black;
    }

    big {
        font-size: larger;
    }

    small {
        font-size: smaller;
    }

    s,
    strike,
    del {
        text-decoration: line-through;
    }

    sub {
        vertical-align: sub;
        font-size: smaller;
    }

    sup {
        vertical-align: super;
        font-size: smaller;
    }

    nobr {
        white-space: nowrap;
    }

    /* states */
    :focus {
        outline: auto 5px -webkit-focus-ring-color;
    }

    /* Read-only text fields do not show a focus ring but do still receive focus */
    html:focus,
    body:focus,
    input[readonly]:focus {
        outline: none;
    }

    embed:focus,
    iframe:focus,
    object:focus {
        outline: none;
    }

    input:focus,
    textarea:focus,
    keygen:focus,
    select:focus {
        outline-offset: -2px;
    }

    input[type='button' i]:focus,
    input[type='checkbox' i]:focus,
    input[type='file' i]:focus,
    input[type='hidden' i]:focus,
    input[type='image' i]:focus,
    input[type='radio' i]:focus,
    input[type='reset' i]:focus,
    input[type='search' i]:focus,
    input[type='submit' i]:focus,
    input[type='file' i]:focus::-webkit-file-upload-button {
        outline-offset: 0;
    }

    a:-webkit-any-link {
        color: -webkit-link;
        text-decoration: underline;
        cursor: auto;
    }

    a:-webkit-any-link:active {
        color: -webkit-activelink;
    }

    /* HTML5 ruby elements */
    ruby,
    rt {
        text-indent: 0;
        /* blocks used for ruby rendering should not trigger this */
    }

    rt {
        line-height: normal;
        -webkit-text-emphasis: none;
    }

    ruby>rt {
        display: block;
        font-size: 50%;
        text-align: start;
    }

    ruby>rp {
        display: none;
    }

    /* other elements */
    noframes {
        display: none;
    }

    frameset,
    frame {
        display: block;
    }

    frameset {
        border-color: inherit;
    }

    iframe {
        border: 2px inset;
    }

    details {
        display: block;
    }

    summary {
        display: block;
    }

    summary::-webkit-details-marker {
        display: inline-block;
        width: 0.66em;
        height: 0.66em;
        -webkit-margin-end: 0.4em;
    }

    template {
        display: none;
    }

    bdi,
    output {
        unicode-bidi: -webkit-isolate;
    }

    bdo {
        unicode-bidi: bidi-override;
    }

    textarea[dir='auto' i] {
        unicode-bidi: -webkit-plaintext;
    }

    dialog:not([open]) {
        display: none;
    }

    dialog {
        position: absolute;
        left: 0;
        right: 0;
        width: -webkit-fit-content;
        height: -webkit-fit-content;
        margin: auto;
        border: solid;
        padding: 1em;
        background: white;
        color: black;
    }

    dialog::backdrop {
        position: fixed;
        top: 0;
        right: 0;
        bottom: 0;
        left: 0;
        background: rgba(0, 0, 0, 0.1);
    }

    /* page */
    @page {
        /* FIXME: Define the right default values for page properties. */
        size: auto;
        margin: auto;
        padding: 0px;
        border-width: 0px;
    }

    /* Disable multicol in printing, since it's not implemented properly. See crbug.com/99358 */
    @media print {
        * {
        -webkit-columns: auto !important;
        }
    }

    /* noscript is handled internally, as it depends on settings. */
    }
    </style>

    <style lang="scss">
    .ck-editor__editable_inline:not(.ck-comment__input *) {
    min-height: 300px;
    }
    </style>

    <style lang="scss">
    /**
    * @license Copyright (c) 2014-2023, CKSource Holding sp. z o.o. All rights reserved.
    * This file is licensed under the terms of the MIT License (see LICENSE.md).
    */

    :root {
    --ck-sample-base-spacing: 2em;
    --ck-sample-color-white: #fff;
    --ck-sample-color-green: #279863;
    --ck-sample-color-blue: #1a9aef;
    --ck-sample-container-width: 1285px;
    --ck-sample-sidebar-width: 350px;
    --ck-sample-editor-min-height: 400px;
    --ck-sample-editor-z-index: 10;
    }

    /* --------- EDITOR STYLES  ---------------------------------------------------------------------------------------- */

    .editor__editable,
    /* Classic build. */
    main .ck-editor[role='application'] .ck.ck-content,
    /* Decoupled document build. */
    .ck.editor__editable[role='textbox'],
    .ck.ck-editor__editable[role='textbox'],
    /* Inline & Balloon build. */
    .ck.editor[role='textbox'] {
    width: 100%;
    background: #fff;
    font-size: 1em;
    line-height: 1.6em;
    min-height: var(--ck-sample-editor-min-height);
    padding: 1.5em 2em;
    }

    .ck.ck-editor__editable {
    background: #fff;
    border: 1px solid hsl(0, 0%, 70%);
    width: 100%;
    }

    /* Because of sidebar `position: relative`, Edge is overriding the outline of a focused editor. */
    .ck.ck-editor__editable {
    position: relative;
    z-index: var(--ck-sample-editor-z-index);
    }

    .editor-container {
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    position: relative;
    width: 100%;
    justify-content: center;
    }

    .editor-container--with-sidebar>.ck.ck-editor {
    width: calc(100% - var(--ck-sample-sidebar-width));
    }

    /* --------- DECOUPLED (DOCUMENT) BUILD. ---------------------------------------------*/
    body[data-editor='DecoupledEditor'] .document-editor__toolbar {
    width: 100%;
    }

    body[data-editor='DecoupledEditor'] .collaboration-demo__editable,
    body[data-editor='DecoupledEditor'] .row-editor .editor {
    /* A pixel is added for each of the border. */
    width: calc(21cm + 2px);
    min-height: calc(29.7cm + 2px);
    /* To avoid having extra scrolls inside the editor container. */
    height: fit-content;
    padding: 2cm 1.2cm;
    margin: 2.5rem;
    border: 1px hsl(0, 0%, 82.7%) solid;
    background-color: var(--ck-sample-color-white);
    box-shadow: 0 0 5px hsla(0, 0%, 0%, 0.1);
    box-sizing: border-box;
    }

    body[data-editor='DecoupledEditor'] .row-editor {
    display: flex;
    position: relative;
    justify-content: center;
    overflow-y: auto;
    background-color: #f2f2f2;
    border: 1px solid hsl(0, 0%, 77%);
    /* Limit the max-height of the editor to avoid scrolling from bottom to top to see the toolbar. */
    max-height: 700px;
    }

    body[data-editor='DecoupledEditor'] .sidebar {
    background: transparent;
    border: 0;
    box-shadow: none;
    }

    /* --------- COMMENTS & TRACK CHANGES FEATURE ---------------------------------------------------------------------- */
    .sidebar {
    padding: 0 15px;
    position: relative;
    min-width: var(--ck-sample-sidebar-width);
    max-width: var(--ck-sample-sidebar-width);
    font-size: 20px;
    border: 1px solid hsl(0, 0%, 77%);
    background: hsl(0, 0%, 98%);
    border-left: 0;
    overflow: hidden;
    min-height: 100%;
    flex-grow: 1;
    }

    /* Do not inherit styles related to the editable editor content. See line 25.*/
    .sidebar .ck-content[role='textbox'],
    .ck.ck-annotation-wrapper .ck-content[role='textbox'] {
    min-height: unset;
    width: unset;
    padding: 0;
    background: transparent;
    }

    .sidebar.narrow {
    min-width: 60px;
    flex-grow: 0;
    }

    .sidebar.hidden {
    display: none !important;
    }

    #sidebar-display-toggle {
    position: absolute;
    z-index: 1;
    width: 30px;
    height: 30px;
    text-align: center;
    left: 15px;
    top: 30px;
    border: 0;
    padding: 0;
    color: hsl(0, 0%, 50%);
    transition: 250ms ease color;
    background-color: transparent;
    }

    #sidebar-display-toggle:hover {
    color: hsl(0, 0%, 30%);
    cursor: pointer;
    }

    #sidebar-display-toggle:focus,
    #sidebar-display-toggle:active {
    outline: none;
    border: 1px solid #a9d29d;
    }

    #sidebar-display-toggle svg {
    fill: currentColor;
    }

    /* --------- COLLABORATION FEATURES (USERS) ------------------------------------------------------------------------ */
    .row-presence {
    width: 100%;
    border: 1px solid hsl(0, 0%, 77%);
    border-bottom: 0;
    background: hsl(0, 0%, 98%);
    padding: var(--ck-spacing-small);

    /* Make `border-bottom` as `box-shadow` to not overlap with the editor border. */
    box-shadow: 0 1px 0 0 hsl(0, 0%, 77%);

    /* Make `z-index` bigger than `.editor` to properly display tooltips. */
    z-index: 20;
    }

    .ck.ck-presence-list {
    flex: 1;
    padding: 1.25rem 0.75rem;
    }

    .presence .ck.ck-presence-list__counter {
    order: 2;
    margin-left: var(--ck-spacing-large);
    }

    /* --------- REAL TIME COLLABORATION FEATURES (SHARE TOPBAR CONTAINER) --------------------------------------------- */
    .collaboration-demo__row {
    display: flex;
    position: relative;
    justify-content: center;
    overflow-y: auto;
    background-color: #f2f2f2;
    border: 1px solid hsl(0, 0%, 77%);
    }

    body[data-editor='InlineEditor'] .collaboration-demo__row {
    border: 0;
    }

    .collaboration-demo__container {
    max-width: var(--ck-sample-container-width);
    margin: 0 auto;
    padding: 1.25rem;
    }

    .presence,
    .collaboration-demo__row {
    transition: 0.2s opacity;
    }

    .collaboration-demo__topbar {
    background: #fff;
    border: 1px solid var(--ck-color-toolbar-border);
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 0;
    border-radius: 4px 4px 0 0;
    }

    .collaboration-demo__topbar .btn {
    margin-right: 1em;
    outline-offset: 2px;
    outline-width: 2px;
    background-color: var(--ck-sample-color-blue);
    }

    .collaboration-demo__topbar .btn:focus,
    .collaboration-demo__topbar .btn:hover {
    border-color: var(--ck-sample-color-blue);
    }

    .collaboration-demo__share {
    display: flex;
    align-items: center;
    padding: 1.25rem 0.75rem;
    }

    .collaboration-demo__share-description p {
    margin: 0;
    font-weight: bold;
    font-size: 0.9em;
    }

    .collaboration-demo__share input {
    height: auto;
    font-size: 0.9em;
    min-width: 220px;
    margin: 0 10px;
    border-radius: 4px;
    border: 1px solid var(--ck-color-toolbar-border);
    }

    .collaboration-demo__share button,
    .collaboration-demo__share input {
    height: 40px;
    padding: 5px 10px;
    }

    .collaboration-demo__share button {
    position: relative;
    }

    .collaboration-demo__share button:focus {
    outline: none;
    }

    .collaboration-demo__share button[data-tooltip]::before,
    .collaboration-demo__share button[data-tooltip]::after {
    position: absolute;
    visibility: hidden;
    opacity: 0;
    pointer-events: none;
    transition: all 0.15s cubic-bezier(0.5, 1, 0.25, 1);
    z-index: 1;
    }

    .collaboration-demo__share button[data-tooltip]::before {
    content: attr(data-tooltip);
    padding: 5px 15px;
    border-radius: 3px;
    background: #111;
    color: #fff;
    text-align: center;
    font-size: 11px;
    top: 100%;
    left: 50%;
    margin-top: 5px;
    transform: translateX(-50%);
    }

    .collaboration-demo__share button[data-tooltip]::after {
    content: '';
    border: 5px solid transparent;
    width: 0;
    font-size: 0;
    line-height: 0;
    top: 100%;
    left: 50%;
    transform: translateX(-50%);
    border-bottom: 5px solid #111;
    border-top: none;
    }

    .collaboration-demo__share button[data-tooltip]:hover:before,
    .collaboration-demo__share button[data-tooltip]:hover:after {
    visibility: visible;
    opacity: 1;
    }

    .collaboration-demo--ready {
    overflow: visible;
    height: auto;
    }

    .collaboration-demo--ready .presence,
    .collaboration-demo--ready .collaboration-demo__row {
    opacity: 1;
    }

    /* --------- PAGINATION FEATURE ------------------------------------------------------------------------------------ */

    /* Pagination view line must be stacked at least at the same level as the editor,
    otherwise it will be hidden underneath. */
    .ck.ck-pagination-view-line {
    z-index: var(--ck-sample-editor-z-index);
    }

    /* --------- REVISION HISTORY FEATURE ------------------------------------------------------------------------------ */

    .revision-viewer-container {
    display: none;
    max-width: 100%;
    word-wrap: break-word;
    }

    .revision-viewer-sidebar {
    position: relative;
    min-width: 310px;
    overflow: hidden;
    background: var(--ck-color-toolbar-background);
    border: 1px solid var(--ck-color-toolbar-border);
    margin-left: -1px;
    }

    /* A case when Pagination and Revision History features are enabled in the editor. */
    /* Move the square with page number from the Pagination plugin to the left side, so that it does not cover the RH sidebar. */
    body[data-revision-history='true'] .ck.ck-pagination-view-line::after {
    transform: translateX(-100%) !important;
    left: -1px !important;
    right: unset !important;
    }

    /* --------- DOCUMENT OUTLINE FEATURE ------------------------------------------------------------------------------ */

    .document-outline-container {
    max-height: 80vh;
    overflow-y: auto;
    margin-bottom: 1em;
    }

    .document-outline-container .ck.ck-document-outline {
    min-height: 100%;
    border: 1px solid var(--ck-color-base-border);
    background-color: hsl(0, 0%, 96%);
    }

    .ck-editor {

    /* --------- SAMPLE GENERIC STYLES (not related to CKEditor) ------------------------------------------------------- */
    a {
        color: #38a5ee;
    }

    header .centered {
        display: flex;
        flex-flow: row nowrap;
        justify-content: space-between;
        align-items: center;
        min-height: 8em;
    }

    header h1 a {
        font-size: 20px;
        display: flex;
        align-items: center;
        color: #2d3a4a;
        text-decoration: none;
    }

    header h1 img {
        display: block;
        height: 64px;
    }

    header nav ul {
        margin: 0;
        padding: 0;
        list-style-type: none;
    }

    header nav ul li {
        display: inline-block;
    }

    header nav ul li+li {
        margin-left: 1em;
    }

    header nav ul li a {
        font-weight: bold;
        text-decoration: none;
        color: #2d3a4a;
    }

    header nav ul li a:hover {
        text-decoration: underline;
    }

    main .message {
        padding: 0 0 var(--ck-sample-base-spacing);
        background: var(--ck-sample-color-green);
        color: var(--ck-sample-color-white);
    }

    main .message::after {
        content: '';
        z-index: -1;
        display: block;
        height: 10em;
        width: 100%;
        background: var(--ck-sample-color-green);
        position: absolute;
        left: 0;
    }

    main .message h2 {
        position: relative;
        padding-top: 1em;
        font-size: 2em;
    }

    .centered {
        max-width: var(--ck-sample-container-width);
        margin: 0 auto;
        padding: 0 var(--ck-sample-base-spacing);
    }

    .row {
        display: flex;
        position: relative;
    }

    .btn {
        cursor: pointer;
        padding: 8px 16px;
        font-size: 1rem;
        user-select: none;
        border-radius: 4px;
        transition: color 0.2s ease-in-out, background-color 0.2s ease-in-out,
        border-color 0.2s ease-in-out, opacity 0.2s ease-in-out;
        background-color: var(--ck-sample-color-button-blue);
        border-color: var(--ck-sample-color-button-blue);
        color: var(--ck-sample-color-white);
        display: inline-block;
    }

    .btn--tiny {
        padding: 6px 12px;
        font-size: 0.8rem;
    }

    footer {
        margin: calc(2 * var(--ck-sample-base-spacing)) var(--ck-sample-base-spacing);
        font-size: 0.8em;
        text-align: center;
        color: rgba(0, 0, 0, 0.4);
    }

    /* --------- RWD --------------------------------------------------------------------------------------------------- */
    @media screen and (max-width: 800px) {
        :root {
        --ck-sample-base-spacing: 1em;
        }

        header h1 {
        width: 100%;
        }

        header h1 img {
        height: 40px;
        }

        header nav ul {
        text-align: right;
        }

        main .message h2 {
        font-size: 1.5em;
        }
    }
    }
    </style>

    <style>
    .ck-hidden {
    display: none !important;
    }

    .ck-reset_all :not(.ck-reset_all-excluded *),
    .ck.ck-reset,
    .ck.ck-reset_all {
    box-sizing: border-box;
    height: auto;
    position: static;
    width: auto;
    }

    :root {
    --ck-z-default: 1;
    --ck-z-modal: calc(var(--ck-z-default) + 999);
    }

    .ck-transitions-disabled,
    .ck-transitions-disabled * {
    transition: none !important;
    }

    :root {
    --ck-powered-by-line-height: 10px;
    --ck-powered-by-padding-vertical: 2px;
    --ck-powered-by-padding-horizontal: 4px;
    --ck-powered-by-text-color: #4f4f4f;
    --ck-powered-by-border-radius: var(--ck-border-radius);
    --ck-powered-by-background: #fff;
    --ck-powered-by-border-color: var(--ck-color-focus-border);
    }

    .ck.ck-balloon-panel.ck-powered-by-balloon {
    --ck-border-radius: var(--ck-powered-by-border-radius);
    background: var(--ck-powered-by-background);
    box-shadow: none;
    min-height: unset;
    z-index: calc(var(--ck-z-modal) - 1);
    }

    .ck.ck-balloon-panel.ck-powered-by-balloon .ck.ck-powered-by {
    line-height: var(--ck-powered-by-line-height);
    }

    .ck.ck-balloon-panel.ck-powered-by-balloon .ck.ck-powered-by a {
    align-items: center;
    cursor: pointer;
    display: flex;
    filter: grayscale(80%);
    line-height: var(--ck-powered-by-line-height);
    opacity: 0.66;
    padding: var(--ck-powered-by-padding-vertical) var(--ck-powered-by-padding-horizontal);
    }

    .ck.ck-balloon-panel.ck-powered-by-balloon .ck.ck-powered-by .ck-powered-by__label {
    color: var(--ck-powered-by-text-color);
    cursor: pointer;
    font-size: 7.5px;
    font-weight: 700;
    letter-spacing: -0.2px;
    line-height: normal;
    margin-right: 4px;
    padding-left: 2px;
    text-transform: uppercase;
    }

    .ck.ck-balloon-panel.ck-powered-by-balloon .ck.ck-powered-by .ck-icon {
    cursor: pointer;
    display: block;
    }

    .ck.ck-balloon-panel.ck-powered-by-balloon .ck.ck-powered-by:hover a {
    filter: grayscale(0);
    opacity: 1;
    }

    .ck.ck-balloon-panel.ck-powered-by-balloon[class*='position_inside'] {
    border-color: transparent;
    }

    .ck.ck-balloon-panel.ck-powered-by-balloon[class*='position_border'] {
    border: var(--ck-focus-ring);
    border-color: var(--ck-powered-by-border-color);
    }

    :root {
    --ck-color-base-foreground: #fafafa;
    --ck-color-base-background: #fff;
    --ck-color-base-border: #ccced1;
    --ck-color-base-action: #53a336;
    --ck-color-base-focus: #6cb5f9;
    --ck-color-base-text: #333;
    --ck-color-base-active: #2977ff;
    --ck-color-base-active-focus: #0d65ff;
    --ck-color-base-error: #db3700;
    --ck-color-focus-border-coordinates: 218, 81.8%, 56.9%;
    --ck-color-focus-border: hsl(var(--ck-color-focus-border-coordinates));
    --ck-color-focus-outer-shadow: #cae1fc;
    --ck-color-focus-disabled-shadow: rgba(119, 186, 248, 0.3);
    --ck-color-focus-error-shadow: rgba(255, 64, 31, 0.3);
    --ck-color-text: var(--ck-color-base-text);
    --ck-color-shadow-drop: rgba(0, 0, 0, 0.15);
    --ck-color-shadow-drop-active: rgba(0, 0, 0, 0.2);
    --ck-color-shadow-inner: rgba(0, 0, 0, 0.1);
    --ck-color-button-default-background: transparent;
    --ck-color-button-default-hover-background: #f0f0f0;
    --ck-color-button-default-active-background: #f0f0f0;
    --ck-color-button-default-disabled-background: transparent;
    --ck-color-button-on-background: #f0f7ff;
    --ck-color-button-on-hover-background: #dbecff;
    --ck-color-button-on-active-background: #dbecff;
    --ck-color-button-on-disabled-background: #f0f2f4;
    --ck-color-button-on-color: #2977ff;
    --ck-color-button-action-background: var(--ck-color-base-action);
    --ck-color-button-action-hover-background: #4d9d30;
    --ck-color-button-action-active-background: #4d9d30;
    --ck-color-button-action-disabled-background: #7ec365;
    --ck-color-button-action-text: var(--ck-color-base-background);
    --ck-color-button-save: #008a00;
    --ck-color-button-cancel: #db3700;
    --ck-color-switch-button-off-background: #939393;
    --ck-color-switch-button-off-hover-background: #7d7d7d;
    --ck-color-switch-button-on-background: var(--ck-color-button-action-background);
    --ck-color-switch-button-on-hover-background: #4d9d30;
    --ck-color-switch-button-inner-background: var(--ck-color-base-background);
    --ck-color-switch-button-inner-shadow: rgba(0, 0, 0, 0.1);
    --ck-color-dropdown-panel-background: var(--ck-color-base-background);
    --ck-color-dropdown-panel-border: var(--ck-color-base-border);
    --ck-color-input-background: var(--ck-color-base-background);
    --ck-color-input-border: var(--ck-color-base-border);
    --ck-color-input-error-border: var(--ck-color-base-error);
    --ck-color-input-text: var(--ck-color-base-text);
    --ck-color-input-disabled-background: #f2f2f2;
    --ck-color-input-disabled-border: var(--ck-color-base-border);
    --ck-color-input-disabled-text: #757575;
    --ck-color-list-background: var(--ck-color-base-background);
    --ck-color-list-button-hover-background: var(--ck-color-button-default-hover-background);
    --ck-color-list-button-on-background: var(--ck-color-button-on-color);
    --ck-color-list-button-on-background-focus: var(--ck-color-button-on-color);
    --ck-color-list-button-on-text: var(--ck-color-base-background);
    --ck-color-panel-background: var(--ck-color-base-background);
    --ck-color-panel-border: var(--ck-color-base-border);
    --ck-color-toolbar-background: var(--ck-color-base-background);
    --ck-color-toolbar-border: var(--ck-color-base-border);
    --ck-color-tooltip-background: var(--ck-color-base-text);
    --ck-color-tooltip-text: var(--ck-color-base-background);
    --ck-color-engine-placeholder-text: #707070;
    --ck-color-upload-bar-background: #6cb5f9;
    --ck-color-link-default: #0000f0;
    --ck-color-link-selected-background: rgba(31, 176, 255, 0.1);
    --ck-color-link-fake-selection: rgba(31, 176, 255, 0.3);
    --ck-color-highlight-background: #ff0;
    --ck-color-light-red: #fcc;
    --ck-disabled-opacity: 0.5;
    --ck-focus-outer-shadow-geometry: 0 0 0 3px;
    --ck-focus-outer-shadow: var(--ck-focus-outer-shadow-geometry) var(--ck-color-focus-outer-shadow);
    --ck-focus-disabled-outer-shadow: var(--ck-focus-outer-shadow-geometry) var(--ck-color-focus-disabled-shadow);
    --ck-focus-error-outer-shadow: var(--ck-focus-outer-shadow-geometry) var(--ck-color-focus-error-shadow);
    --ck-focus-ring: 1px solid var(--ck-color-focus-border);
    --ck-font-size-base: 13px;
    --ck-line-height-base: 1.84615;
    --ck-font-face: Helvetica, Arial, Tahoma, Verdana, Sans-Serif;
    --ck-font-size-tiny: 0.7em;
    --ck-font-size-small: 0.75em;
    --ck-font-size-normal: 1em;
    --ck-font-size-big: 1.4em;
    --ck-font-size-large: 1.8em;
    --ck-ui-component-min-height: 2.3em;
    }

    .ck-reset_all :not(.ck-reset_all-excluded *),
    .ck.ck-reset,
    .ck.ck-reset_all {
    word-wrap: break-word;
    background: transparent;
    border: 0;
    margin: 0;
    padding: 0;
    text-decoration: none;
    transition: none;
    vertical-align: middle;
    }

    .ck-reset_all :not(.ck-reset_all-excluded *),
    .ck.ck-reset_all {
    border-collapse: collapse;
    color: var(--ck-color-text);
    cursor: auto;
    float: none;
    font: normal normal normal var(--ck-font-size-base) / var(--ck-line-height-base) var(--ck-font-face);
    text-align: left;
    white-space: nowrap;
    }

    .ck-reset_all .ck-rtl :not(.ck-reset_all-excluded *) {
    text-align: right;
    }

    .ck-reset_all iframe:not(.ck-reset_all-excluded *) {
    vertical-align: inherit;
    }

    .ck-reset_all textarea:not(.ck-reset_all-excluded *) {
    white-space: pre-wrap;
    }

    .ck-reset_all input[type='password']:not(.ck-reset_all-excluded *),
    .ck-reset_all input[type='text']:not(.ck-reset_all-excluded *),
    .ck-reset_all textarea:not(.ck-reset_all-excluded *) {
    cursor: text;
    }

    .ck-reset_all input[type='password'][disabled]:not(.ck-reset_all-excluded *),
    .ck-reset_all input[type='text'][disabled]:not(.ck-reset_all-excluded *),
    .ck-reset_all textarea[disabled]:not(.ck-reset_all-excluded *) {
    cursor: default;
    }

    .ck-reset_all fieldset:not(.ck-reset_all-excluded *) {
    border: 2px groove #dfdee3;
    padding: 10px;
    }

    .ck-reset_all button:not(.ck-reset_all-excluded *)::-moz-focus-inner {
    border: 0;
    padding: 0;
    }

    .ck[dir='rtl'],
    .ck[dir='rtl'] .ck {
    text-align: right;
    }

    :root {
    --ck-border-radius: 2px;
    --ck-inner-shadow: 2px 2px 3px var(--ck-color-shadow-inner) inset;
    --ck-drop-shadow: 0 1px 2px 1px var(--ck-color-shadow-drop);
    --ck-drop-shadow-active: 0 3px 6px 1px var(--ck-color-shadow-drop-active);
    --ck-spacing-unit: 0.6em;
    --ck-spacing-large: calc(var(--ck-spacing-unit) * 1.5);
    --ck-spacing-standard: var(--ck-spacing-unit);
    --ck-spacing-medium: calc(var(--ck-spacing-unit) * 0.8);
    --ck-spacing-small: calc(var(--ck-spacing-unit) * 0.5);
    --ck-spacing-tiny: calc(var(--ck-spacing-unit) * 0.3);
    --ck-spacing-extra-tiny: calc(var(--ck-spacing-unit) * 0.16);
    }

    .ck.ck-icon {
    vertical-align: middle;
    }

    :root {
    --ck-icon-size: calc(var(--ck-line-height-base) * var(--ck-font-size-normal));
    }

    .ck.ck-icon {
    font-size: 0.8333350694em;
    height: var(--ck-icon-size);
    width: var(--ck-icon-size);
    will-change: transform;
    }

    .ck.ck-icon,
    .ck.ck-icon * {
    cursor: inherit;
    }

    .ck.ck-icon.ck-icon_inherit-color,
    .ck.ck-icon.ck-icon_inherit-color * {
    color: inherit;
    }

    .ck.ck-icon.ck-icon_inherit-color :not([fill]) {
    fill: currentColor;
    }

    .ck.ck-button,
    a.ck.ck-button {
    align-items: center;
    display: inline-flex;
    position: relative;
    -moz-user-select: none;
    -webkit-user-select: none;
    -ms-user-select: none;
    user-select: none;
    }

    [dir='ltr'] .ck.ck-button,
    [dir='ltr'] a.ck.ck-button {
    justify-content: left;
    }

    [dir='rtl'] .ck.ck-button,
    [dir='rtl'] a.ck.ck-button {
    justify-content: right;
    }

    .ck.ck-button .ck-button__label,
    a.ck.ck-button .ck-button__label {
    display: none;
    }

    .ck.ck-button.ck-button_with-text .ck-button__label,
    a.ck.ck-button.ck-button_with-text .ck-button__label {
    display: inline-block;
    }

    .ck.ck-button:not(.ck-button_with-text),
    a.ck.ck-button:not(.ck-button_with-text) {
    justify-content: center;
    }

    .ck.ck-button,
    a.ck.ck-button {
    background: var(--ck-color-button-default-background);
    }

    .ck.ck-button:not(.ck-disabled):hover,
    a.ck.ck-button:not(.ck-disabled):hover {
    background: var(--ck-color-button-default-hover-background);
    }

    .ck.ck-button:not(.ck-disabled):active,
    a.ck.ck-button:not(.ck-disabled):active {
    background: var(--ck-color-button-default-active-background);
    }

    .ck.ck-button.ck-disabled,
    a.ck.ck-button.ck-disabled {
    background: var(--ck-color-button-default-disabled-background);
    }

    .ck.ck-button,
    a.ck.ck-button {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-button,
    .ck-rounded-corners a.ck.ck-button,
    .ck.ck-button.ck-rounded-corners,
    a.ck.ck-button.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    }

    .ck.ck-button,
    a.ck.ck-button {
    -webkit-appearance: none;
    border: 1px solid transparent;
    cursor: default;
    font-size: inherit;
    line-height: 1;
    min-height: var(--ck-ui-component-min-height);
    min-width: var(--ck-ui-component-min-height);
    padding: var(--ck-spacing-tiny);
    text-align: center;
    transition: box-shadow 0.2s ease-in-out, border 0.2s ease-in-out;
    vertical-align: middle;
    white-space: nowrap;
    }

    .ck.ck-button:active,
    .ck.ck-button:focus,
    a.ck.ck-button:active,
    a.ck.ck-button:focus {
    border: var(--ck-focus-ring);
    box-shadow: var(--ck-focus-outer-shadow), 0 0;
    outline: none;
    }

    .ck.ck-button .ck-button__icon use,
    .ck.ck-button .ck-button__icon use *,
    a.ck.ck-button .ck-button__icon use,
    a.ck.ck-button .ck-button__icon use * {
    color: inherit;
    }

    .ck.ck-button .ck-button__label,
    a.ck.ck-button .ck-button__label {
    color: inherit;
    cursor: inherit;
    font-size: inherit;
    font-weight: inherit;
    vertical-align: middle;
    }

    [dir='ltr'] .ck.ck-button .ck-button__label,
    [dir='ltr'] a.ck.ck-button .ck-button__label {
    text-align: left;
    }

    [dir='rtl'] .ck.ck-button .ck-button__label,
    [dir='rtl'] a.ck.ck-button .ck-button__label {
    text-align: right;
    }

    .ck.ck-button .ck-button__keystroke,
    a.ck.ck-button .ck-button__keystroke {
    color: inherit;
    }

    [dir='ltr'] .ck.ck-button .ck-button__keystroke,
    [dir='ltr'] a.ck.ck-button .ck-button__keystroke {
    margin-left: var(--ck-spacing-large);
    }

    [dir='rtl'] .ck.ck-button .ck-button__keystroke,
    [dir='rtl'] a.ck.ck-button .ck-button__keystroke {
    margin-right: var(--ck-spacing-large);
    }

    .ck.ck-button .ck-button__keystroke,
    a.ck.ck-button .ck-button__keystroke {
    font-weight: 700;
    opacity: 0.7;
    }

    .ck.ck-button.ck-disabled:active,
    .ck.ck-button.ck-disabled:focus,
    a.ck.ck-button.ck-disabled:active,
    a.ck.ck-button.ck-disabled:focus {
    box-shadow: var(--ck-focus-disabled-outer-shadow), 0 0;
    }

    .ck.ck-button.ck-disabled .ck-button__icon,
    .ck.ck-button.ck-disabled .ck-button__label,
    a.ck.ck-button.ck-disabled .ck-button__icon,
    a.ck.ck-button.ck-disabled .ck-button__label {
    opacity: var(--ck-disabled-opacity);
    }

    .ck.ck-button.ck-disabled .ck-button__keystroke,
    a.ck.ck-button.ck-disabled .ck-button__keystroke {
    opacity: 0.3;
    }

    .ck.ck-button.ck-button_with-text,
    a.ck.ck-button.ck-button_with-text {
    padding: var(--ck-spacing-tiny) var(--ck-spacing-standard);
    }

    [dir='ltr'] .ck.ck-button.ck-button_with-text .ck-button__icon,
    [dir='ltr'] a.ck.ck-button.ck-button_with-text .ck-button__icon {
    margin-left: calc(var(--ck-spacing-small) * -1);
    margin-right: var(--ck-spacing-small);
    }

    [dir='rtl'] .ck.ck-button.ck-button_with-text .ck-button__icon,
    [dir='rtl'] a.ck.ck-button.ck-button_with-text .ck-button__icon {
    margin-left: var(--ck-spacing-small);
    margin-right: calc(var(--ck-spacing-small) * -1);
    }

    .ck.ck-button.ck-button_with-keystroke .ck-button__label,
    a.ck.ck-button.ck-button_with-keystroke .ck-button__label {
    flex-grow: 1;
    }

    .ck.ck-button.ck-on,
    a.ck.ck-button.ck-on {
    background: var(--ck-color-button-on-background);
    }

    .ck.ck-button.ck-on:not(.ck-disabled):hover,
    a.ck.ck-button.ck-on:not(.ck-disabled):hover {
    background: var(--ck-color-button-on-hover-background);
    }

    .ck.ck-button.ck-on:not(.ck-disabled):active,
    a.ck.ck-button.ck-on:not(.ck-disabled):active {
    background: var(--ck-color-button-on-active-background);
    }

    .ck.ck-button.ck-on.ck-disabled,
    a.ck.ck-button.ck-on.ck-disabled {
    background: var(--ck-color-button-on-disabled-background);
    }

    .ck.ck-button.ck-on,
    a.ck.ck-button.ck-on {
    color: var(--ck-color-button-on-color);
    }

    .ck.ck-button.ck-button-save,
    a.ck.ck-button.ck-button-save {
    color: var(--ck-color-button-save);
    }

    .ck.ck-button.ck-button-cancel,
    a.ck.ck-button.ck-button-cancel {
    color: var(--ck-color-button-cancel);
    }

    .ck.ck-button-action,
    a.ck.ck-button-action {
    background: var(--ck-color-button-action-background);
    }

    .ck.ck-button-action:not(.ck-disabled):hover,
    a.ck.ck-button-action:not(.ck-disabled):hover {
    background: var(--ck-color-button-action-hover-background);
    }

    .ck.ck-button-action:not(.ck-disabled):active,
    a.ck.ck-button-action:not(.ck-disabled):active {
    background: var(--ck-color-button-action-active-background);
    }

    .ck.ck-button-action.ck-disabled,
    a.ck.ck-button-action.ck-disabled {
    background: var(--ck-color-button-action-disabled-background);
    }

    .ck.ck-button-action,
    a.ck.ck-button-action {
    color: var(--ck-color-button-action-text);
    }

    .ck.ck-button-bold,
    a.ck.ck-button-bold {
    font-weight: 700;
    }

    .ck.ck-button.ck-switchbutton .ck-button__toggle,
    .ck.ck-button.ck-switchbutton .ck-button__toggle .ck-button__toggle__inner {
    display: block;
    }

    :root {
    --ck-switch-button-toggle-width: 2.6153846154em;
    --ck-switch-button-toggle-inner-size: calc(1.07692em + 1px);
    --ck-switch-button-translation: calc(var(--ck-switch-button-toggle-width) - var(--ck-switch-button-toggle-inner-size) - 2px);
    --ck-switch-button-inner-hover-shadow: 0 0 0 5px var(--ck-color-switch-button-inner-shadow);
    }

    .ck.ck-button.ck-switchbutton,
    .ck.ck-button.ck-switchbutton.ck-on:active,
    .ck.ck-button.ck-switchbutton.ck-on:focus,
    .ck.ck-button.ck-switchbutton.ck-on:hover,
    .ck.ck-button.ck-switchbutton:active,
    .ck.ck-button.ck-switchbutton:focus,
    .ck.ck-button.ck-switchbutton:hover {
    background: transparent;
    color: inherit;
    }

    [dir='ltr'] .ck.ck-button.ck-switchbutton .ck-button__label {
    margin-right: calc(var(--ck-spacing-large) * 2);
    }

    [dir='rtl'] .ck.ck-button.ck-switchbutton .ck-button__label {
    margin-left: calc(var(--ck-spacing-large) * 2);
    }

    .ck.ck-button.ck-switchbutton .ck-button__toggle {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-button.ck-switchbutton .ck-button__toggle,
    .ck.ck-button.ck-switchbutton .ck-button__toggle.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    }

    [dir='ltr'] .ck.ck-button.ck-switchbutton .ck-button__toggle {
    margin-left: auto;
    }

    [dir='rtl'] .ck.ck-button.ck-switchbutton .ck-button__toggle {
    margin-right: auto;
    }

    .ck.ck-button.ck-switchbutton .ck-button__toggle {
    background: var(--ck-color-switch-button-off-background);
    border: 1px solid transparent;
    transition: background 0.4s ease, box-shadow 0.2s ease-in-out,
        outline 0.2s ease-in-out;
    width: var(--ck-switch-button-toggle-width);
    }

    .ck.ck-button.ck-switchbutton .ck-button__toggle .ck-button__toggle__inner {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-button.ck-switchbutton .ck-button__toggle .ck-button__toggle__inner,
    .ck.ck-button.ck-switchbutton .ck-button__toggle .ck-button__toggle__inner.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    border-radius: calc(var(--ck-border-radius) * 0.5);
    }

    .ck.ck-button.ck-switchbutton .ck-button__toggle .ck-button__toggle__inner {
    background: var(--ck-color-switch-button-inner-background);
    height: var(--ck-switch-button-toggle-inner-size);
    transition: all 0.3s ease;
    width: var(--ck-switch-button-toggle-inner-size);
    }

    .ck.ck-button.ck-switchbutton .ck-button__toggle:hover {
    background: var(--ck-color-switch-button-off-hover-background);
    }

    .ck.ck-button.ck-switchbutton .ck-button__toggle:hover .ck-button__toggle__inner {
    box-shadow: var(--ck-switch-button-inner-hover-shadow);
    }

    .ck.ck-button.ck-switchbutton.ck-disabled .ck-button__toggle {
    opacity: var(--ck-disabled-opacity);
    }

    .ck.ck-button.ck-switchbutton:focus {
    border-color: transparent;
    box-shadow: none;
    outline: none;
    }

    .ck.ck-button.ck-switchbutton:focus .ck-button__toggle {
    box-shadow: 0 0 0 1px var(--ck-color-base-background),
        0 0 0 5px var(--ck-color-focus-outer-shadow);
    outline: var(--ck-focus-ring);
    outline-offset: 1px;
    }

    .ck.ck-button.ck-switchbutton.ck-on .ck-button__toggle {
    background: var(--ck-color-switch-button-on-background);
    }

    .ck.ck-button.ck-switchbutton.ck-on .ck-button__toggle:hover {
    background: var(--ck-color-switch-button-on-hover-background);
    }

    [dir='ltr'] .ck.ck-button.ck-switchbutton.ck-on .ck-button__toggle .ck-button__toggle__inner {
    transform: translateX(var(--ck-switch-button-translation));
    }

    [dir='rtl'] .ck.ck-button.ck-switchbutton.ck-on .ck-button__toggle .ck-button__toggle__inner {
    transform: translateX(calc(var(--ck-switch-button-translation) * -1));
    }

    .ck.ck-color-grid {
    display: grid;
    }

    :root {
    --ck-color-grid-tile-size: 24px;
    --ck-color-color-grid-check-icon: #166fd4;
    }

    .ck.ck-color-grid {
    grid-gap: 5px;
    padding: 8px;
    }

    .ck.ck-color-grid__tile {
    border: 0;
    height: var(--ck-color-grid-tile-size);
    min-height: var(--ck-color-grid-tile-size);
    min-width: var(--ck-color-grid-tile-size);
    padding: 0;
    transition: box-shadow 0.2s ease;
    width: var(--ck-color-grid-tile-size);
    }

    .ck.ck-color-grid__tile.ck-disabled {
    cursor: unset;
    transition: unset;
    }

    .ck.ck-color-grid__tile.ck-color-selector__color-tile_bordered {
    box-shadow: 0 0 0 1px var(--ck-color-base-border);
    }

    .ck.ck-color-grid__tile .ck.ck-icon {
    color: var(--ck-color-color-grid-check-icon);
    display: none;
    }

    .ck.ck-color-grid__tile.ck-on {
    box-shadow: inset 0 0 0 1px var(--ck-color-base-background),
        0 0 0 2px var(--ck-color-base-text);
    }

    .ck.ck-color-grid__tile.ck-on .ck.ck-icon {
    display: block;
    }

    .ck.ck-color-grid__tile.ck-on,
    .ck.ck-color-grid__tile:focus:not(.ck-disabled),
    .ck.ck-color-grid__tile:hover:not(.ck-disabled) {
    border: 0;
    }

    .ck.ck-color-grid__tile:focus:not(.ck-disabled),
    .ck.ck-color-grid__tile:hover:not(.ck-disabled) {
    box-shadow: inset 0 0 0 1px var(--ck-color-base-background),
        0 0 0 2px var(--ck-color-focus-border);
    }

    .ck.ck-color-grid__label {
    padding: 0 var(--ck-spacing-standard);
    }

    .ck.ck-label {
    display: block;
    }

    .ck.ck-voice-label {
    display: none;
    }

    .ck.ck-label {
    font-weight: 700;
    }

    .ck.ck-labeled-field-view>.ck.ck-labeled-field-view__input-wrapper {
    display: flex;
    position: relative;
    }

    .ck.ck-labeled-field-view .ck.ck-label {
    display: block;
    position: absolute;
    }

    :root {
    --ck-labeled-field-view-transition: 0.1s cubic-bezier(0, 0, 0.24, 0.95);
    --ck-labeled-field-empty-unfocused-max-width: 100% - 2 * var(--ck-spacing-medium);
    --ck-labeled-field-label-default-position-x: var(--ck-spacing-medium);
    --ck-labeled-field-label-default-position-y: calc(var(--ck-font-size-base) * 0.6);
    --ck-color-labeled-field-label-background: var(--ck-color-base-background);
    }

    .ck.ck-labeled-field-view {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-labeled-field-view,
    .ck.ck-labeled-field-view.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    }

    .ck.ck-labeled-field-view>.ck.ck-labeled-field-view__input-wrapper {
    width: 100%;
    }

    .ck.ck-labeled-field-view>.ck.ck-labeled-field-view__input-wrapper>.ck.ck-label {
    top: 0;
    }

    [dir='ltr'] .ck.ck-labeled-field-view>.ck.ck-labeled-field-view__input-wrapper>.ck.ck-label {
    left: 0;
    transform: translate(var(--ck-spacing-medium), -6px) scale(0.75);
    transform-origin: 0 0;
    }

    [dir='rtl'] .ck.ck-labeled-field-view>.ck.ck-labeled-field-view__input-wrapper>.ck.ck-label {
    right: 0;
    transform: translate(calc(var(--ck-spacing-medium) * -1), -6px) scale(0.75);
    transform-origin: 100% 0;
    }

    .ck.ck-labeled-field-view>.ck.ck-labeled-field-view__input-wrapper>.ck.ck-label {
    background: var(--ck-color-labeled-field-label-background);
    font-weight: 400;
    line-height: normal;
    max-width: 100%;
    overflow: hidden;
    padding: 0 calc(var(--ck-font-size-tiny) * 0.5);
    pointer-events: none;
    text-overflow: ellipsis;
    transition: transform var(--ck-labeled-field-view-transition),
        padding var(--ck-labeled-field-view-transition),
        background var(--ck-labeled-field-view-transition);
    }

    .ck.ck-labeled-field-view.ck-error .ck-input:not([readonly])+.ck.ck-label,
    .ck.ck-labeled-field-view.ck-error>.ck.ck-labeled-field-view__input-wrapper>.ck.ck-label {
    color: var(--ck-color-base-error);
    }

    .ck.ck-labeled-field-view .ck-labeled-field-view__status {
    font-size: var(--ck-font-size-small);
    margin-top: var(--ck-spacing-small);
    white-space: normal;
    }

    .ck.ck-labeled-field-view .ck-labeled-field-view__status.ck-labeled-field-view__status_error {
    color: var(--ck-color-base-error);
    }

    .ck.ck-labeled-field-view.ck-disabled>.ck.ck-labeled-field-view__input-wrapper>.ck.ck-label,
    .ck.ck-labeled-field-view.ck-labeled-field-view_empty:not(.ck-labeled-field-view_focused)>.ck.ck-labeled-field-view__input-wrapper>.ck.ck-label {
    color: var(--ck-color-input-disabled-text);
    }

    [dir='ltr'] .ck.ck-labeled-field-view.ck-disabled.ck-labeled-field-view_empty:not(.ck-labeled-field-view_placeholder)>.ck.ck-labeled-field-view__input-wrapper>.ck.ck-label,
    [dir='ltr'] .ck.ck-labeled-field-view.ck-labeled-field-view_empty:not(.ck-labeled-field-view_focused):not(.ck-labeled-field-view_placeholder)>.ck.ck-labeled-field-view__input-wrapper>.ck.ck-label {
    transform: translate(var(--ck-labeled-field-label-default-position-x),
        var(--ck-labeled-field-label-default-position-y)) scale(1);
    }

    [dir='rtl'] .ck.ck-labeled-field-view.ck-disabled.ck-labeled-field-view_empty:not(.ck-labeled-field-view_placeholder)>.ck.ck-labeled-field-view__input-wrapper>.ck.ck-label,
    [dir='rtl'] .ck.ck-labeled-field-view.ck-labeled-field-view_empty:not(.ck-labeled-field-view_focused):not(.ck-labeled-field-view_placeholder)>.ck.ck-labeled-field-view__input-wrapper>.ck.ck-label {
    transform: translate(calc(var(--ck-labeled-field-label-default-position-x) * -1),
        var(--ck-labeled-field-label-default-position-y)) scale(1);
    }

    .ck.ck-labeled-field-view.ck-disabled.ck-labeled-field-view_empty:not(.ck-labeled-field-view_placeholder)>.ck.ck-labeled-field-view__input-wrapper>.ck.ck-label,
    .ck.ck-labeled-field-view.ck-labeled-field-view_empty:not(.ck-labeled-field-view_focused):not(.ck-labeled-field-view_placeholder)>.ck.ck-labeled-field-view__input-wrapper>.ck.ck-label {
    background: transparent;
    max-width: calc(var(--ck-labeled-field-empty-unfocused-max-width));
    padding: 0;
    }

    .ck.ck-labeled-field-view>.ck.ck-labeled-field-view__input-wrapper>.ck-dropdown>.ck.ck-button {
    background: transparent;
    }

    .ck.ck-labeled-field-view.ck-labeled-field-view_empty>.ck.ck-labeled-field-view__input-wrapper>.ck-dropdown>.ck-button>.ck-button__label {
    opacity: 0;
    }

    .ck.ck-labeled-field-view.ck-labeled-field-view_empty:not(.ck-labeled-field-view_focused):not(.ck-labeled-field-view_placeholder)>.ck.ck-labeled-field-view__input-wrapper>.ck-dropdown+.ck-label {
    max-width: calc(var(--ck-labeled-field-empty-unfocused-max-width) - var(--ck-dropdown-arrow-size) - var(--ck-spacing-standard));
    }

    :root {
    --ck-input-width: 18em;
    --ck-input-text-width: var(--ck-input-width);
    }

    .ck.ck-input {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-input,
    .ck.ck-input.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    }

    .ck.ck-input {
    background: var(--ck-color-input-background);
    border: 1px solid var(--ck-color-input-border);
    min-height: var(--ck-ui-component-min-height);
    min-width: var(--ck-input-width);
    padding: var(--ck-spacing-extra-tiny) var(--ck-spacing-medium);
    transition: box-shadow 0.1s ease-in-out, border 0.1s ease-in-out;
    }

    .ck.ck-input:focus {
    border: var(--ck-focus-ring);
    box-shadow: var(--ck-focus-outer-shadow), 0 0;
    outline: none;
    }

    .ck.ck-input[readonly] {
    background: var(--ck-color-input-disabled-background);
    border: 1px solid var(--ck-color-input-disabled-border);
    color: var(--ck-color-input-disabled-text);
    }

    .ck.ck-input[readonly]:focus {
    box-shadow: var(--ck-focus-disabled-outer-shadow), 0 0;
    }

    .ck.ck-input.ck-error {
    animation: ck-input-shake 0.3s ease both;
    border-color: var(--ck-color-input-error-border);
    }

    .ck.ck-input.ck-error:focus {
    box-shadow: var(--ck-focus-error-outer-shadow), 0 0;
    }

    @keyframes ck-input-shake {
    20% {
        transform: translateX(-2px);
    }

    40% {
        transform: translateX(2px);
    }

    60% {
        transform: translateX(-1px);
    }

    80% {
        transform: translateX(1px);
    }
    }

    .ck-textarea {
    overflow-x: hidden;
    }

    :root {
    --ck-dropdown-max-width: 75vw;
    }

    .ck.ck-dropdown {
    display: inline-block;
    position: relative;
    }

    .ck.ck-dropdown .ck-dropdown__arrow {
    pointer-events: none;
    z-index: var(--ck-z-default);
    }

    .ck.ck-dropdown .ck-button.ck-dropdown__button {
    width: 100%;
    }

    .ck.ck-dropdown .ck-dropdown__panel {
    display: none;
    max-width: var(--ck-dropdown-max-width);
    position: absolute;
    z-index: var(--ck-z-modal);
    }

    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel-visible {
    display: inline-block;
    }

    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_n,
    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_ne,
    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_nme,
    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_nmw,
    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_nw {
    bottom: 100%;
    }

    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_s,
    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_se,
    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_sme,
    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_smw,
    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_sw {
    bottom: auto;
    top: 100%;
    }

    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_ne,
    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_se {
    left: 0;
    }

    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_nw,
    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_sw {
    right: 0;
    }

    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_n,
    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_s {
    left: 50%;
    transform: translateX(-50%);
    }

    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_nmw,
    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_smw {
    left: 75%;
    transform: translateX(-75%);
    }

    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_nme,
    .ck.ck-dropdown .ck-dropdown__panel.ck-dropdown__panel_sme {
    left: 25%;
    transform: translateX(-25%);
    }

    .ck.ck-toolbar .ck-dropdown__panel {
    z-index: calc(var(--ck-z-modal) + 1);
    }

    :root {
    --ck-dropdown-arrow-size: calc(var(--ck-icon-size) * 0.5);
    }

    .ck.ck-dropdown {
    font-size: inherit;
    }

    .ck.ck-dropdown .ck-dropdown__arrow {
    width: var(--ck-dropdown-arrow-size);
    }

    [dir='ltr'] .ck.ck-dropdown .ck-dropdown__arrow {
    margin-left: var(--ck-spacing-standard);
    right: var(--ck-spacing-standard);
    }

    [dir='rtl'] .ck.ck-dropdown .ck-dropdown__arrow {
    left: var(--ck-spacing-standard);
    margin-right: var(--ck-spacing-small);
    }

    .ck.ck-dropdown.ck-disabled .ck-dropdown__arrow {
    opacity: var(--ck-disabled-opacity);
    }

    [dir='ltr'] .ck.ck-dropdown .ck-button.ck-dropdown__button:not(.ck-button_with-text) {
    padding-left: var(--ck-spacing-small);
    }

    [dir='rtl'] .ck.ck-dropdown .ck-button.ck-dropdown__button:not(.ck-button_with-text) {
    padding-right: var(--ck-spacing-small);
    }

    .ck.ck-dropdown .ck-button.ck-dropdown__button .ck-button__label {
    overflow: hidden;
    text-overflow: ellipsis;
    width: 7em;
    }

    .ck.ck-dropdown .ck-button.ck-dropdown__button.ck-disabled .ck-button__label {
    opacity: var(--ck-disabled-opacity);
    }

    .ck.ck-dropdown .ck-button.ck-dropdown__button.ck-on {
    border-bottom-left-radius: 0;
    border-bottom-right-radius: 0;
    }

    .ck.ck-dropdown .ck-button.ck-dropdown__button.ck-dropdown__button_label-width_auto .ck-button__label {
    width: auto;
    }

    .ck.ck-dropdown .ck-button.ck-dropdown__button.ck-off:active,
    .ck.ck-dropdown .ck-button.ck-dropdown__button.ck-on:active {
    box-shadow: none;
    }

    .ck.ck-dropdown .ck-button.ck-dropdown__button.ck-off:active:focus,
    .ck.ck-dropdown .ck-button.ck-dropdown__button.ck-on:active:focus {
    box-shadow: var(--ck-focus-outer-shadow), 0 0;
    }

    .ck.ck-dropdown__panel {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-dropdown__panel,
    .ck.ck-dropdown__panel.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    }

    .ck.ck-dropdown__panel {
    background: var(--ck-color-dropdown-panel-background);
    border: 1px solid var(--ck-color-dropdown-panel-border);
    bottom: 0;
    box-shadow: var(--ck-drop-shadow), 0 0;
    min-width: 100%;
    }

    .ck.ck-dropdown__panel.ck-dropdown__panel_se {
    border-top-left-radius: 0;
    }

    .ck.ck-dropdown__panel.ck-dropdown__panel_sw {
    border-top-right-radius: 0;
    }

    .ck.ck-dropdown__panel.ck-dropdown__panel_ne {
    border-bottom-left-radius: 0;
    }

    .ck.ck-dropdown__panel.ck-dropdown__panel_nw {
    border-bottom-right-radius: 0;
    }

    .ck.ck-dropdown__panel:focus {
    outline: none;
    }

    .ck .ck-placeholder,
    .ck.ck-placeholder {
    position: relative;
    }

    .ck .ck-placeholder:before,
    .ck.ck-placeholder:before {
    content: attr(data-placeholder);
    left: 0;
    pointer-events: none;
    position: absolute;
    right: 0;
    }

    .ck.ck-read-only .ck-placeholder:before {
    display: none;
    }

    .ck.ck-reset_all .ck-placeholder {
    position: relative;
    }

    .ck .ck-placeholder:before,
    .ck.ck-placeholder:before {
    color: var(--ck-color-engine-placeholder-text);
    cursor: text;
    }

    .ck.ck-editor__editable span[data-ck-unsafe-element] {
    display: none;
    }

    .ck.ck-toolbar {
    align-items: center;
    display: flex;
    flex-flow: row nowrap;
    -moz-user-select: none;
    -webkit-user-select: none;
    -ms-user-select: none;
    user-select: none;
    }

    .ck.ck-toolbar>.ck-toolbar__items {
    align-items: center;
    display: flex;
    flex-flow: row wrap;
    flex-grow: 1;
    }

    .ck.ck-toolbar .ck.ck-toolbar__separator {
    display: inline-block;
    }

    .ck.ck-toolbar .ck.ck-toolbar__separator:first-child,
    .ck.ck-toolbar .ck.ck-toolbar__separator:last-child {
    display: none;
    }

    .ck.ck-toolbar .ck-toolbar__line-break {
    flex-basis: 100%;
    }

    .ck.ck-toolbar.ck-toolbar_grouping>.ck-toolbar__items {
    flex-wrap: nowrap;
    }

    .ck.ck-toolbar.ck-toolbar_vertical>.ck-toolbar__items {
    flex-direction: column;
    }

    .ck.ck-toolbar.ck-toolbar_floating>.ck-toolbar__items {
    flex-wrap: nowrap;
    }

    .ck.ck-toolbar>.ck.ck-toolbar__grouped-dropdown>.ck-dropdown__button .ck-dropdown__arrow {
    display: none;
    }

    .ck.ck-toolbar {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-toolbar,
    .ck.ck-toolbar.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    }

    .ck.ck-toolbar {
    background: var(--ck-color-toolbar-background);
    border: 1px solid var(--ck-color-toolbar-border);
    padding: 0 var(--ck-spacing-small);
    }

    .ck.ck-toolbar .ck.ck-toolbar__separator {
    align-self: stretch;
    background: var(--ck-color-toolbar-border);
    margin-bottom: var(--ck-spacing-small);
    margin-top: var(--ck-spacing-small);
    min-width: 1px;
    width: 1px;
    }

    .ck.ck-toolbar .ck-toolbar__line-break {
    height: 0;
    }

    .ck.ck-toolbar>.ck-toolbar__items> :not(.ck-toolbar__line-break) {
    margin-right: var(--ck-spacing-small);
    }

    .ck.ck-toolbar>.ck-toolbar__items:empty+.ck.ck-toolbar__separator {
    display: none;
    }

    .ck.ck-toolbar>.ck-toolbar__items> :not(.ck-toolbar__line-break),
    .ck.ck-toolbar>.ck.ck-toolbar__grouped-dropdown {
    margin-bottom: var(--ck-spacing-small);
    margin-top: var(--ck-spacing-small);
    }

    .ck.ck-toolbar.ck-toolbar_vertical {
    padding: 0;
    }

    .ck.ck-toolbar.ck-toolbar_vertical>.ck-toolbar__items>.ck {
    border-radius: 0;
    margin: 0;
    width: 100%;
    }

    .ck.ck-toolbar.ck-toolbar_compact {
    padding: 0;
    }

    .ck.ck-toolbar.ck-toolbar_compact>.ck-toolbar__items>* {
    margin: 0;
    }

    .ck.ck-toolbar.ck-toolbar_compact>.ck-toolbar__items> :not(:first-child):not(:last-child) {
    border-radius: 0;
    }

    .ck.ck-toolbar>.ck.ck-toolbar__grouped-dropdown>.ck.ck-button.ck-dropdown__button {
    padding-left: var(--ck-spacing-tiny);
    }

    .ck.ck-toolbar .ck-toolbar__nested-toolbar-dropdown>.ck-dropdown__panel {
    min-width: auto;
    }

    .ck.ck-toolbar .ck-toolbar__nested-toolbar-dropdown>.ck-button>.ck-button__label {
    max-width: 7em;
    width: auto;
    }

    .ck.ck-toolbar:focus {
    outline: none;
    }

    .ck-toolbar-container .ck.ck-toolbar {
    border: 0;
    }

    .ck.ck-toolbar[dir='rtl']>.ck-toolbar__items>.ck,
    [dir='rtl'] .ck.ck-toolbar>.ck-toolbar__items>.ck {
    margin-right: 0;
    }

    .ck.ck-toolbar[dir='rtl']:not(.ck-toolbar_compact)>.ck-toolbar__items>.ck,
    [dir='rtl'] .ck.ck-toolbar:not(.ck-toolbar_compact)>.ck-toolbar__items>.ck {
    margin-left: var(--ck-spacing-small);
    }

    .ck.ck-toolbar[dir='rtl']>.ck-toolbar__items>.ck:last-child,
    [dir='rtl'] .ck.ck-toolbar>.ck-toolbar__items>.ck:last-child {
    margin-left: 0;
    }

    .ck.ck-toolbar.ck-toolbar_compact[dir='rtl']>.ck-toolbar__items>.ck:first-child,
    [dir='rtl'] .ck.ck-toolbar.ck-toolbar_compact>.ck-toolbar__items>.ck:first-child {
    border-bottom-left-radius: 0;
    border-top-left-radius: 0;
    }

    .ck.ck-toolbar.ck-toolbar_compact[dir='rtl']>.ck-toolbar__items>.ck:last-child,
    [dir='rtl'] .ck.ck-toolbar.ck-toolbar_compact>.ck-toolbar__items>.ck:last-child {
    border-bottom-right-radius: 0;
    border-top-right-radius: 0;
    }

    .ck.ck-toolbar.ck-toolbar_grouping[dir='rtl']>.ck-toolbar__items:not(:empty):not(:only-child),
    .ck.ck-toolbar[dir='rtl']>.ck.ck-toolbar__separator,
    [dir='rtl'] .ck.ck-toolbar.ck-toolbar_grouping>.ck-toolbar__items:not(:empty):not(:only-child),
    [dir='rtl'] .ck.ck-toolbar>.ck.ck-toolbar__separator {
    margin-left: var(--ck-spacing-small);
    }

    .ck.ck-toolbar[dir='ltr']>.ck-toolbar__items>.ck:last-child,
    [dir='ltr'] .ck.ck-toolbar>.ck-toolbar__items>.ck:last-child {
    margin-right: 0;
    }

    .ck.ck-toolbar.ck-toolbar_compact[dir='ltr']>.ck-toolbar__items>.ck:first-child,
    [dir='ltr'] .ck.ck-toolbar.ck-toolbar_compact>.ck-toolbar__items>.ck:first-child {
    border-bottom-right-radius: 0;
    border-top-right-radius: 0;
    }

    .ck.ck-toolbar.ck-toolbar_compact[dir='ltr']>.ck-toolbar__items>.ck:last-child,
    [dir='ltr'] .ck.ck-toolbar.ck-toolbar_compact>.ck-toolbar__items>.ck:last-child {
    border-bottom-left-radius: 0;
    border-top-left-radius: 0;
    }

    .ck.ck-toolbar.ck-toolbar_grouping[dir='ltr']>.ck-toolbar__items:not(:empty):not(:only-child),
    .ck.ck-toolbar[dir='ltr']>.ck.ck-toolbar__separator,
    [dir='ltr'] .ck.ck-toolbar.ck-toolbar_grouping>.ck-toolbar__items:not(:empty):not(:only-child),
    [dir='ltr'] .ck.ck-toolbar>.ck.ck-toolbar__separator {
    margin-right: var(--ck-spacing-small);
    }

    .ck.ck-list {
    display: flex;
    flex-direction: column;
    -moz-user-select: none;
    -webkit-user-select: none;
    -ms-user-select: none;
    user-select: none;
    }

    .ck.ck-list .ck-list__item,
    .ck.ck-list .ck-list__separator {
    display: block;
    }

    .ck.ck-list .ck-list__item> :focus {
    position: relative;
    z-index: var(--ck-z-default);
    }

    :root {
    --ck-list-button-padding: calc(var(--ck-line-height-base) * 0.2 * var(--ck-font-size-base)) calc(var(--ck-line-height-base) * 0.4 * var(--ck-font-size-base));
    }

    .ck.ck-list {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-list,
    .ck.ck-list.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    }

    .ck.ck-list {
    background: var(--ck-color-list-background);
    list-style-type: none;
    }

    .ck.ck-list__item {
    cursor: default;
    min-width: 12em;
    }

    .ck.ck-list__item .ck-button {
    border-radius: 0;
    min-height: unset;
    width: 100%;
    }

    [dir='ltr'] .ck.ck-list__item .ck-button {
    text-align: left;
    }

    [dir='rtl'] .ck.ck-list__item .ck-button {
    text-align: right;
    }

    .ck.ck-list__item .ck-button {
    padding: var(--ck-list-button-padding);
    }

    .ck.ck-list__item .ck-button .ck-button__label {
    line-height: calc(var(--ck-line-height-base) * 1.2 * var(--ck-font-size-base));
    }

    .ck.ck-list__item .ck-button:active {
    box-shadow: none;
    }

    .ck.ck-list__item .ck-button.ck-on {
    background: var(--ck-color-list-button-on-background);
    color: var(--ck-color-list-button-on-text);
    }

    .ck.ck-list__item .ck-button.ck-on:active {
    box-shadow: none;
    }

    .ck.ck-list__item .ck-button.ck-on:hover:not(.ck-disabled) {
    background: var(--ck-color-list-button-on-background-focus);
    }

    .ck.ck-list__item .ck-button.ck-on:focus:not(.ck-switchbutton):not(.ck-disabled) {
    border-color: var(--ck-color-base-background);
    }

    .ck.ck-list__item .ck-button:hover:not(.ck-disabled) {
    background: var(--ck-color-list-button-hover-background);
    }

    .ck.ck-list__item .ck-switchbutton.ck-on {
    background: var(--ck-color-list-background);
    color: inherit;
    }

    .ck.ck-list__item .ck-switchbutton.ck-on:hover:not(.ck-disabled) {
    background: var(--ck-color-list-button-hover-background);
    color: inherit;
    }

    .ck-list .ck-list__group {
    padding-top: var(--ck-spacing-medium);

    :not(.ck-hidden)~& {
        border-top: 1px solid var(--ck-color-base-border);
    }
    }

    .ck-list .ck-list__group>.ck-label {
    font-size: 11px;
    font-weight: 700;
    padding: var(--ck-spacing-medium) var(--ck-spacing-medium) 0 var(--ck-spacing-medium);
    }

    .ck.ck-list__separator {
    background: var(--ck-color-base-border);
    height: 1px;
    width: 100%;
    }

    .ck.ck-splitbutton {
    font-size: inherit;
    }

    .ck.ck-splitbutton .ck-splitbutton__action:focus {
    z-index: calc(var(--ck-z-default) + 1);
    }

    :root {
    --ck-color-split-button-hover-background: #ebebeb;
    --ck-color-split-button-hover-border: #b3b3b3;
    }

    [dir='ltr'] .ck.ck-splitbutton.ck-splitbutton_open>.ck-splitbutton__action,
    [dir='ltr'] .ck.ck-splitbutton:hover>.ck-splitbutton__action {
    border-bottom-right-radius: unset;
    border-top-right-radius: unset;
    }

    [dir='rtl'] .ck.ck-splitbutton.ck-splitbutton_open>.ck-splitbutton__action,
    [dir='rtl'] .ck.ck-splitbutton:hover>.ck-splitbutton__action {
    border-bottom-left-radius: unset;
    border-top-left-radius: unset;
    }

    .ck.ck-splitbutton>.ck-splitbutton__arrow {
    min-width: unset;
    }

    [dir='ltr'] .ck.ck-splitbutton>.ck-splitbutton__arrow {
    border-bottom-left-radius: unset;
    border-top-left-radius: unset;
    }

    [dir='rtl'] .ck.ck-splitbutton>.ck-splitbutton__arrow {
    border-bottom-right-radius: unset;
    border-top-right-radius: unset;
    }

    .ck.ck-splitbutton>.ck-splitbutton__arrow svg {
    width: var(--ck-dropdown-arrow-size);
    }

    .ck.ck-splitbutton>.ck-splitbutton__arrow:not(:focus) {
    border-bottom-width: 0;
    border-top-width: 0;
    }

    .ck.ck-splitbutton.ck-splitbutton_open>.ck-button:not(.ck-on):not(.ck-disabled):not(:hover),
    .ck.ck-splitbutton:hover>.ck-button:not(.ck-on):not(.ck-disabled):not(:hover) {
    background: var(--ck-color-split-button-hover-background);
    }

    .ck.ck-splitbutton.ck-splitbutton_open>.ck-splitbutton__arrow:not(.ck-disabled):after,
    .ck.ck-splitbutton:hover>.ck-splitbutton__arrow:not(.ck-disabled):after {
    background-color: var(--ck-color-split-button-hover-border);
    content: '';
    height: 100%;
    position: absolute;
    width: 1px;
    }

    .ck.ck-splitbutton.ck-splitbutton_open>.ck-splitbutton__arrow:focus:after,
    .ck.ck-splitbutton:hover>.ck-splitbutton__arrow:focus:after {
    --ck-color-split-button-hover-border: var(--ck-color-focus-border);
    }

    [dir='ltr'] .ck.ck-splitbutton.ck-splitbutton_open>.ck-splitbutton__arrow:not(.ck-disabled):after,
    [dir='ltr'] .ck.ck-splitbutton:hover>.ck-splitbutton__arrow:not(.ck-disabled):after {
    left: -1px;
    }

    [dir='rtl'] .ck.ck-splitbutton.ck-splitbutton_open>.ck-splitbutton__arrow:not(.ck-disabled):after,
    [dir='rtl'] .ck.ck-splitbutton:hover>.ck-splitbutton__arrow:not(.ck-disabled):after {
    right: -1px;
    }

    .ck.ck-splitbutton.ck-splitbutton_open {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-splitbutton.ck-splitbutton_open,
    .ck.ck-splitbutton.ck-splitbutton_open.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    }

    .ck-rounded-corners .ck.ck-splitbutton.ck-splitbutton_open>.ck-splitbutton__action,
    .ck.ck-splitbutton.ck-splitbutton_open.ck-rounded-corners>.ck-splitbutton__action {
    border-bottom-left-radius: 0;
    }

    .ck-rounded-corners .ck.ck-splitbutton.ck-splitbutton_open>.ck-splitbutton__arrow,
    .ck.ck-splitbutton.ck-splitbutton_open.ck-rounded-corners>.ck-splitbutton__arrow {
    border-bottom-right-radius: 0;
    }

    :root {
    --ck-toolbar-dropdown-max-width: 60vw;
    }

    .ck.ck-toolbar-dropdown>.ck-dropdown__panel {
    max-width: var(--ck-toolbar-dropdown-max-width);
    width: max-content;
    }

    .ck.ck-toolbar-dropdown>.ck-dropdown__panel .ck-button:focus {
    z-index: calc(var(--ck-z-default) + 1);
    }

    .ck.ck-toolbar-dropdown .ck-toolbar {
    border: 0;
    }

    .ck.ck-dropdown .ck-dropdown__panel .ck-list {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-dropdown .ck-dropdown__panel .ck-list,
    .ck.ck-dropdown .ck-dropdown__panel .ck-list.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    border-top-left-radius: 0;
    }

    .ck.ck-dropdown .ck-dropdown__panel .ck-list .ck-list__item:first-child .ck-button {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-dropdown .ck-dropdown__panel .ck-list .ck-list__item:first-child .ck-button,
    .ck.ck-dropdown .ck-dropdown__panel .ck-list .ck-list__item:first-child .ck-button.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    border-bottom-left-radius: 0;
    border-bottom-right-radius: 0;
    border-top-left-radius: 0;
    }

    .ck.ck-dropdown .ck-dropdown__panel .ck-list .ck-list__item:last-child .ck-button {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-dropdown .ck-dropdown__panel .ck-list .ck-list__item:last-child .ck-button,
    .ck.ck-dropdown .ck-dropdown__panel .ck-list .ck-list__item:last-child .ck-button.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    border-top-left-radius: 0;
    border-top-right-radius: 0;
    }

    .color-picker-hex-input {
    width: max-content;
    }

    .color-picker-hex-input .ck.ck-input {
    min-width: unset;
    }

    .ck.ck-color-picker__row {
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-between;
    margin: var(--ck-spacing-large) 0 0;
    width: unset;
    }

    .ck.ck-color-picker__row .ck.ck-labeled-field-view {
    padding-top: unset;
    }

    .ck.ck-color-picker__row .ck.ck-input-text {
    width: unset;
    }

    .ck.ck-color-picker__row .ck-color-picker__hash-view {
    padding-right: var(--ck-spacing-medium);
    padding-top: var(--ck-spacing-tiny);
    }

    .ck.ck-color-selector .ck-color-grids-fragment .ck-button.ck-color-selector__color-picker,
    .ck.ck-color-selector .ck-color-grids-fragment .ck-button.ck-color-selector__remove-color {
    align-items: center;
    display: flex;
    }

    [dir='rtl'] .ck.ck-color-selector .ck-color-grids-fragment .ck-button.ck-color-selector__color-picker,
    [dir='rtl'] .ck.ck-color-selector .ck-color-grids-fragment .ck-button.ck-color-selector__remove-color {
    justify-content: flex-start;
    }

    .ck.ck-color-selector .ck-color-picker-fragment .ck.ck-color-selector_action-bar {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    }

    .ck.ck-color-selector .ck-color-picker-fragment .ck.ck-color-selector_action-bar .ck-button-cancel,
    .ck.ck-color-selector .ck-color-picker-fragment .ck.ck-color-selector_action-bar .ck-button-save {
    flex: 1;
    }

    .ck.ck-color-selector .ck-color-grids-fragment .ck-button.ck-color-selector__color-picker,
    .ck.ck-color-selector .ck-color-grids-fragment .ck-button.ck-color-selector__remove-color {
    width: 100%;
    }

    .ck.ck-color-selector .ck-color-grids-fragment .ck-button.ck-color-selector__color-picker {
    border-bottom-left-radius: 0;
    border-bottom-right-radius: 0;
    padding: calc(var(--ck-spacing-standard) / 2) var(--ck-spacing-standard);
    }

    .ck.ck-color-selector .ck-color-grids-fragment .ck-button.ck-color-selector__color-picker:not(:focus) {
    border-top: 1px solid var(--ck-color-base-border);
    }

    [dir='ltr'] .ck.ck-color-selector .ck-color-grids-fragment .ck-button.ck-color-selector__color-picker .ck.ck-icon {
    margin-right: var(--ck-spacing-standard);
    }

    [dir='rtl'] .ck.ck-color-selector .ck-color-grids-fragment .ck-button.ck-color-selector__color-picker .ck.ck-icon {
    margin-left: var(--ck-spacing-standard);
    }

    .ck.ck-color-selector .ck-color-grids-fragment label.ck.ck-color-grid__label {
    font-weight: unset;
    }

    .ck.ck-color-selector .ck-color-picker-fragment .ck.ck-color-picker {
    padding: 8px;
    }

    .ck.ck-color-selector .ck-color-picker-fragment .ck.ck-color-picker .hex-color-picker {
    height: 100px;
    min-width: 180px;
    }

    .ck.ck-color-selector .ck-color-picker-fragment .ck.ck-color-picker .hex-color-picker::part(saturation) {
    border-radius: var(--ck-border-radius) var(--ck-border-radius) 0 0;
    }

    .ck.ck-color-selector .ck-color-picker-fragment .ck.ck-color-picker .hex-color-picker::part(hue) {
    border-radius: 0 0 var(--ck-border-radius) var(--ck-border-radius);
    }

    .ck.ck-color-selector .ck-color-picker-fragment .ck.ck-color-picker .hex-color-picker::part(hue-pointer),
    .ck.ck-color-selector .ck-color-picker-fragment .ck.ck-color-picker .hex-color-picker::part(saturation-pointer) {
    height: 15px;
    width: 15px;
    }

    .ck.ck-color-selector .ck-color-picker-fragment .ck.ck-color-selector_action-bar {
    padding: 0 8px 8px;
    }

    :root {
    --ck-balloon-panel-arrow-z-index: calc(var(--ck-z-default) - 3);
    }

    .ck.ck-balloon-panel {
    display: none;
    position: absolute;
    z-index: var(--ck-z-modal);
    }

    .ck.ck-balloon-panel.ck-balloon-panel_with-arrow:after,
    .ck.ck-balloon-panel.ck-balloon-panel_with-arrow:before {
    content: '';
    position: absolute;
    }

    .ck.ck-balloon-panel.ck-balloon-panel_with-arrow:before {
    z-index: var(--ck-balloon-panel-arrow-z-index);
    }

    .ck.ck-balloon-panel.ck-balloon-panel_with-arrow:after {
    z-index: calc(var(--ck-balloon-panel-arrow-z-index) + 1);
    }

    .ck.ck-balloon-panel[class*='arrow_n']:before {
    z-index: var(--ck-balloon-panel-arrow-z-index);
    }

    .ck.ck-balloon-panel[class*='arrow_n']:after {
    z-index: calc(var(--ck-balloon-panel-arrow-z-index) + 1);
    }

    .ck.ck-balloon-panel[class*='arrow_s']:before {
    z-index: var(--ck-balloon-panel-arrow-z-index);
    }

    .ck.ck-balloon-panel[class*='arrow_s']:after {
    z-index: calc(var(--ck-balloon-panel-arrow-z-index) + 1);
    }

    .ck.ck-balloon-panel.ck-balloon-panel_visible {
    display: block;
    }

    :root {
    --ck-balloon-border-width: 1px;
    --ck-balloon-arrow-offset: 2px;
    --ck-balloon-arrow-height: 10px;
    --ck-balloon-arrow-half-width: 8px;
    --ck-balloon-arrow-drop-shadow: 0 2px 2px var(--ck-color-shadow-drop);
    }

    .ck.ck-balloon-panel {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-balloon-panel,
    .ck.ck-balloon-panel.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    }

    .ck.ck-balloon-panel {
    background: var(--ck-color-panel-background);
    border: var(--ck-balloon-border-width) solid var(--ck-color-panel-border);
    box-shadow: var(--ck-drop-shadow), 0 0;
    min-height: 15px;
    }

    .ck.ck-balloon-panel.ck-balloon-panel_with-arrow:after,
    .ck.ck-balloon-panel.ck-balloon-panel_with-arrow:before {
    border-style: solid;
    height: 0;
    width: 0;
    }

    .ck.ck-balloon-panel[class*='arrow_n']:after,
    .ck.ck-balloon-panel[class*='arrow_n']:before {
    border-width: 0 var(--ck-balloon-arrow-half-width) var(--ck-balloon-arrow-height) var(--ck-balloon-arrow-half-width);
    }

    .ck.ck-balloon-panel[class*='arrow_n']:before {
    border-color: transparent transparent var(--ck-color-panel-border) transparent;
    margin-top: calc(var(--ck-balloon-border-width) * -1);
    }

    .ck.ck-balloon-panel[class*='arrow_n']:after {
    border-color: transparent transparent var(--ck-color-panel-background) transparent;
    margin-top: calc(var(--ck-balloon-arrow-offset) - var(--ck-balloon-border-width));
    }

    .ck.ck-balloon-panel[class*='arrow_s']:after,
    .ck.ck-balloon-panel[class*='arrow_s']:before {
    border-width: var(--ck-balloon-arrow-height) var(--ck-balloon-arrow-half-width) 0 var(--ck-balloon-arrow-half-width);
    }

    .ck.ck-balloon-panel[class*='arrow_s']:before {
    border-color: var(--ck-color-panel-border) transparent transparent;
    filter: drop-shadow(var(--ck-balloon-arrow-drop-shadow));
    margin-bottom: calc(var(--ck-balloon-border-width) * -1);
    }

    .ck.ck-balloon-panel[class*='arrow_s']:after {
    border-color: var(--ck-color-panel-background) transparent transparent transparent;
    margin-bottom: calc(var(--ck-balloon-arrow-offset) - var(--ck-balloon-border-width));
    }

    .ck.ck-balloon-panel[class*='arrow_e']:after,
    .ck.ck-balloon-panel[class*='arrow_e']:before {
    border-width: var(--ck-balloon-arrow-half-width) 0 var(--ck-balloon-arrow-half-width) var(--ck-balloon-arrow-height);
    }

    .ck.ck-balloon-panel[class*='arrow_e']:before {
    border-color: transparent transparent transparent var(--ck-color-panel-border);
    margin-right: calc(var(--ck-balloon-border-width) * -1);
    }

    .ck.ck-balloon-panel[class*='arrow_e']:after {
    border-color: transparent transparent transparent var(--ck-color-panel-background);
    margin-right: calc(var(--ck-balloon-arrow-offset) - var(--ck-balloon-border-width));
    }

    .ck.ck-balloon-panel[class*='arrow_w']:after,
    .ck.ck-balloon-panel[class*='arrow_w']:before {
    border-width: var(--ck-balloon-arrow-half-width) var(--ck-balloon-arrow-height) var(--ck-balloon-arrow-half-width) 0;
    }

    .ck.ck-balloon-panel[class*='arrow_w']:before {
    border-color: transparent var(--ck-color-panel-border) transparent transparent;
    margin-left: calc(var(--ck-balloon-border-width) * -1);
    }

    .ck.ck-balloon-panel[class*='arrow_w']:after {
    border-color: transparent var(--ck-color-panel-background) transparent transparent;
    margin-left: calc(var(--ck-balloon-arrow-offset) - var(--ck-balloon-border-width));
    }

    .ck.ck-balloon-panel.ck-balloon-panel_arrow_n:after,
    .ck.ck-balloon-panel.ck-balloon-panel_arrow_n:before {
    left: 50%;
    margin-left: calc(var(--ck-balloon-arrow-half-width) * -1);
    top: calc(var(--ck-balloon-arrow-height) * -1);
    }

    .ck.ck-balloon-panel.ck-balloon-panel_arrow_nw:after,
    .ck.ck-balloon-panel.ck-balloon-panel_arrow_nw:before {
    left: calc(var(--ck-balloon-arrow-half-width) * 2);
    top: calc(var(--ck-balloon-arrow-height) * -1);
    }

    .ck.ck-balloon-panel.ck-balloon-panel_arrow_ne:after,
    .ck.ck-balloon-panel.ck-balloon-panel_arrow_ne:before {
    right: calc(var(--ck-balloon-arrow-half-width) * 2);
    top: calc(var(--ck-balloon-arrow-height) * -1);
    }

    .ck.ck-balloon-panel.ck-balloon-panel_arrow_s:after,
    .ck.ck-balloon-panel.ck-balloon-panel_arrow_s:before {
    bottom: calc(var(--ck-balloon-arrow-height) * -1);
    left: 50%;
    margin-left: calc(var(--ck-balloon-arrow-half-width) * -1);
    }

    .ck.ck-balloon-panel.ck-balloon-panel_arrow_sw:after,
    .ck.ck-balloon-panel.ck-balloon-panel_arrow_sw:before {
    bottom: calc(var(--ck-balloon-arrow-height) * -1);
    left: calc(var(--ck-balloon-arrow-half-width) * 2);
    }

    .ck.ck-balloon-panel.ck-balloon-panel_arrow_se:after,
    .ck.ck-balloon-panel.ck-balloon-panel_arrow_se:before {
    bottom: calc(var(--ck-balloon-arrow-height) * -1);
    right: calc(var(--ck-balloon-arrow-half-width) * 2);
    }

    .ck.ck-balloon-panel.ck-balloon-panel_arrow_sme:after,
    .ck.ck-balloon-panel.ck-balloon-panel_arrow_sme:before {
    bottom: calc(var(--ck-balloon-arrow-height) * -1);
    margin-right: calc(var(--ck-balloon-arrow-half-width) * 2);
    right: 25%;
    }

    .ck.ck-balloon-panel.ck-balloon-panel_arrow_smw:after,
    .ck.ck-balloon-panel.ck-balloon-panel_arrow_smw:before {
    bottom: calc(var(--ck-balloon-arrow-height) * -1);
    left: 25%;
    margin-left: calc(var(--ck-balloon-arrow-half-width) * 2);
    }

    .ck.ck-balloon-panel.ck-balloon-panel_arrow_nme:after,
    .ck.ck-balloon-panel.ck-balloon-panel_arrow_nme:before {
    margin-right: calc(var(--ck-balloon-arrow-half-width) * 2);
    right: 25%;
    top: calc(var(--ck-balloon-arrow-height) * -1);
    }

    .ck.ck-balloon-panel.ck-balloon-panel_arrow_nmw:after,
    .ck.ck-balloon-panel.ck-balloon-panel_arrow_nmw:before {
    left: 25%;
    margin-left: calc(var(--ck-balloon-arrow-half-width) * 2);
    top: calc(var(--ck-balloon-arrow-height) * -1);
    }

    .ck.ck-balloon-panel.ck-balloon-panel_arrow_e:after,
    .ck.ck-balloon-panel.ck-balloon-panel_arrow_e:before {
    margin-top: calc(var(--ck-balloon-arrow-half-width) * -1);
    right: calc(var(--ck-balloon-arrow-height) * -1);
    top: 50%;
    }

    .ck.ck-balloon-panel.ck-balloon-panel_arrow_w:after,
    .ck.ck-balloon-panel.ck-balloon-panel_arrow_w:before {
    left: calc(var(--ck-balloon-arrow-height) * -1);
    margin-top: calc(var(--ck-balloon-arrow-half-width) * -1);
    top: 50%;
    }

    .ck.ck-balloon-panel.ck-tooltip {
    --ck-balloon-border-width: 0px;
    --ck-balloon-arrow-offset: 0px;
    --ck-balloon-arrow-half-width: 4px;
    --ck-balloon-arrow-height: 4px;
    --ck-tooltip-text-padding: 4px;
    --ck-color-panel-background: var(--ck-color-tooltip-background);
    padding: 0 var(--ck-spacing-medium);
    pointer-events: none;
    z-index: calc(var(--ck-z-modal) + 100);
    }

    .ck.ck-balloon-panel.ck-tooltip .ck-tooltip__text {
    color: var(--ck-color-tooltip-text);
    font-size: 0.9em;
    line-height: 1.5;
    }

    .ck.ck-balloon-panel.ck-tooltip.ck-tooltip_multi-line .ck-tooltip__text {
    display: inline-block;
    padding: var(--ck-tooltip-text-padding) 0;
    white-space: break-spaces;
    }

    .ck.ck-balloon-panel.ck-tooltip {
    box-shadow: none;
    }

    .ck.ck-balloon-panel.ck-tooltip:before {
    display: none;
    }

    .ck.ck-aria-live-announcer {
    left: -10000px;
    position: absolute;
    top: -10000px;
    }

    :root {
    --ck-color-editable-blur-selection: #d9d9d9;
    }

    .ck.ck-editor__editable:not(.ck-editor__nested-editable) {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-editor__editable:not(.ck-editor__nested-editable),
    .ck.ck-editor__editable.ck-rounded-corners:not(.ck-editor__nested-editable) {
    border-radius: var(--ck-border-radius);
    }

    .ck.ck-editor__editable.ck-focused:not(.ck-editor__nested-editable) {
    border: var(--ck-focus-ring);
    box-shadow: var(--ck-inner-shadow), 0 0;
    outline: none;
    }

    .ck.ck-editor__editable_inline {
    border: 1px solid transparent;
    overflow: auto;
    padding: 0 var(--ck-spacing-standard);
    }

    .ck.ck-editor__editable_inline[dir='ltr'] {
    text-align: left;
    }

    .ck.ck-editor__editable_inline[dir='rtl'] {
    text-align: right;
    }

    .ck.ck-editor__editable_inline> :first-child {
    margin-top: var(--ck-spacing-large);
    }

    .ck.ck-editor__editable_inline> :last-child {
    margin-bottom: var(--ck-spacing-large);
    }

    .ck.ck-editor__editable_inline.ck-blurred ::selection {
    background: var(--ck-color-editable-blur-selection);
    }

    .ck.ck-balloon-panel.ck-toolbar-container[class*='arrow_n']:after {
    border-bottom-color: var(--ck-color-panel-background);
    }

    .ck.ck-balloon-panel.ck-toolbar-container[class*='arrow_s']:after {
    border-top-color: var(--ck-color-panel-background);
    }

    .ck.ck-form__header {
    align-items: center;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-between;
    }

    .ck.ck-form__header h2.ck-form__header__label {
    flex-grow: 1;
    }

    :root {
    --ck-form-header-height: 38px;
    }

    .ck.ck-form__header {
    border-bottom: 1px solid var(--ck-color-base-border);
    height: var(--ck-form-header-height);
    line-height: var(--ck-form-header-height);
    padding: var(--ck-spacing-small) var(--ck-spacing-large);
    }

    [dir='ltr'] .ck.ck-form__header .ck-icon {
    margin-right: var(--ck-spacing-medium);
    }

    [dir='rtl'] .ck.ck-form__header .ck-icon {
    margin-left: var(--ck-spacing-medium);
    }

    .ck.ck-form__header .ck-form__header__label {
    font-weight: 700;
    }

    .ck .ck-balloon-rotator__navigation {
    align-items: center;
    display: flex;
    justify-content: center;
    }

    .ck .ck-balloon-rotator__content .ck-toolbar {
    justify-content: center;
    }

    .ck .ck-balloon-rotator__navigation {
    background: var(--ck-color-toolbar-background);
    border-bottom: 1px solid var(--ck-color-toolbar-border);
    padding: 0 var(--ck-spacing-small);
    }

    .ck .ck-balloon-rotator__navigation>* {
    margin-bottom: var(--ck-spacing-small);
    margin-right: var(--ck-spacing-small);
    margin-top: var(--ck-spacing-small);
    }

    .ck .ck-balloon-rotator__navigation .ck-balloon-rotator__counter {
    margin-left: var(--ck-spacing-small);
    margin-right: var(--ck-spacing-standard);
    }

    .ck .ck-balloon-rotator__content .ck.ck-annotation-wrapper {
    box-shadow: none;
    }

    .ck .ck-fake-panel {
    position: absolute;
    z-index: calc(var(--ck-z-modal) - 1);
    }

    .ck .ck-fake-panel div {
    position: absolute;
    }

    .ck .ck-fake-panel div:first-child {
    z-index: 2;
    }

    .ck .ck-fake-panel div:nth-child(2) {
    z-index: 1;
    }

    :root {
    --ck-balloon-fake-panel-offset-horizontal: 6px;
    --ck-balloon-fake-panel-offset-vertical: 6px;
    }

    .ck .ck-fake-panel div {
    background: var(--ck-color-panel-background);
    border: 1px solid var(--ck-color-panel-border);
    border-radius: var(--ck-border-radius);
    box-shadow: var(--ck-drop-shadow), 0 0;
    height: 100%;
    min-height: 15px;
    width: 100%;
    }

    .ck .ck-fake-panel div:first-child {
    margin-left: var(--ck-balloon-fake-panel-offset-horizontal);
    margin-top: var(--ck-balloon-fake-panel-offset-vertical);
    }

    .ck .ck-fake-panel div:nth-child(2) {
    margin-left: calc(var(--ck-balloon-fake-panel-offset-horizontal) * 2);
    margin-top: calc(var(--ck-balloon-fake-panel-offset-vertical) * 2);
    }

    .ck .ck-fake-panel div:nth-child(3) {
    margin-left: calc(var(--ck-balloon-fake-panel-offset-horizontal) * 3);
    margin-top: calc(var(--ck-balloon-fake-panel-offset-vertical) * 3);
    }

    .ck .ck-balloon-panel_arrow_s+.ck-fake-panel,
    .ck .ck-balloon-panel_arrow_se+.ck-fake-panel,
    .ck .ck-balloon-panel_arrow_sw+.ck-fake-panel {
    --ck-balloon-fake-panel-offset-vertical: -6px;
    }

    .ck.ck-sticky-panel .ck-sticky-panel__content_sticky {
    position: fixed;
    top: 0;
    z-index: var(--ck-z-modal);
    }

    .ck.ck-sticky-panel .ck-sticky-panel__content_sticky_bottom-limit {
    position: absolute;
    top: auto;
    }

    .ck.ck-sticky-panel .ck-sticky-panel__content_sticky {
    border-top-left-radius: 0;
    border-top-right-radius: 0;
    border-width: 0 1px 1px;
    box-shadow: var(--ck-drop-shadow), 0 0;
    }

    .ck.ck-search>.ck-labeled-field-view>.ck-labeled-field-view__input-wrapper>.ck-icon {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    }

    [dir='ltr'] .ck.ck-search>.ck-labeled-field-view>.ck-labeled-field-view__input-wrapper>.ck-icon {
    left: var(--ck-spacing-medium);
    }

    [dir='rtl'] .ck.ck-search>.ck-labeled-field-view>.ck-labeled-field-view__input-wrapper>.ck-icon {
    right: var(--ck-spacing-medium);
    }

    .ck.ck-search>.ck-labeled-field-view .ck-search__reset {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    }

    .ck.ck-search>.ck-search__results>.ck-search__info>span:first-child {
    display: block;
    }

    .ck.ck-search>.ck-search__results>.ck-search__info:not(.ck-hidden)~* {
    display: none;
    }

    :root {
    --ck-search-field-view-horizontal-spacing: calc(var(--ck-icon-size) + var(--ck-spacing-medium));
    }

    .ck.ck-search>.ck-labeled-field-view .ck-input {
    width: 100%;
    }

    .ck.ck-search>.ck-labeled-field-view.ck-search__query_with-icon {
    --ck-labeled-field-label-default-position-x: var(--ck-search-field-view-horizontal-spacing);
    }

    .ck.ck-search>.ck-labeled-field-view.ck-search__query_with-icon>.ck-labeled-field-view__input-wrapper>.ck-icon {
    opacity: 0.5;
    pointer-events: none;
    }

    .ck.ck-search>.ck-labeled-field-view.ck-search__query_with-icon .ck-input {
    width: 100%;
    }

    [dir='ltr'] .ck.ck-search>.ck-labeled-field-view.ck-search__query_with-icon .ck-input,
    [dir='rtl'] .ck.ck-search>.ck-labeled-field-view.ck-search__query_with-icon .ck-input:not(.ck-input-text_empty) {
    padding-left: var(--ck-search-field-view-horizontal-spacing);
    }

    .ck.ck-search>.ck-labeled-field-view.ck-search__query_with-reset {
    --ck-labeled-field-empty-unfocused-max-width: 100% - 2 * var(--ck-search-field-view-horizontal-spacing);
    }

    .ck.ck-search>.ck-labeled-field-view.ck-search__query_with-reset.ck-labeled-field-view_empty {
    --ck-labeled-field-empty-unfocused-max-width: 100% - var(--ck-search-field-view-horizontal-spacing) - var(--ck-spacing-medium);
    }

    .ck.ck-search>.ck-labeled-field-view.ck-search__query_with-reset .ck-search__reset {
    background: none;
    min-height: auto;
    min-width: auto;
    opacity: 0.5;
    padding: 0;
    }

    [dir='ltr'] .ck.ck-search>.ck-labeled-field-view.ck-search__query_with-reset .ck-search__reset {
    right: var(--ck-spacing-medium);
    }

    [dir='rtl'] .ck.ck-search>.ck-labeled-field-view.ck-search__query_with-reset .ck-search__reset {
    left: var(--ck-spacing-medium);
    }

    .ck.ck-search>.ck-labeled-field-view.ck-search__query_with-reset .ck-search__reset:hover {
    opacity: 1;
    }

    .ck.ck-search>.ck-labeled-field-view.ck-search__query_with-reset .ck-input {
    width: 100%;
    }

    [dir='ltr'] .ck.ck-search>.ck-labeled-field-view.ck-search__query_with-reset .ck-input:not(.ck-input-text_empty),
    [dir='rtl'] .ck.ck-search>.ck-labeled-field-view.ck-search__query_with-reset .ck-input {
    padding-right: var(--ck-search-field-view-horizontal-spacing);
    }

    .ck.ck-search>.ck-search__results {
    min-width: 100%;
    }

    .ck.ck-search>.ck-search__results>.ck-search__info {
    padding: var(--ck-spacing-medium) var(--ck-spacing-large);
    width: 100%;
    }

    .ck.ck-search>.ck-search__results>.ck-search__info * {
    white-space: normal;
    }

    .ck.ck-search>.ck-search__results>.ck-search__info>span:first-child {
    font-weight: 700;
    }

    .ck.ck-search>.ck-search__results>.ck-search__info>span:last-child {
    margin-top: var(--ck-spacing-medium);
    }

    .ck.ck-autocomplete {
    position: relative;
    }

    .ck.ck-autocomplete>.ck-search__results {
    position: absolute;
    z-index: var(--ck-z-modal);
    }

    .ck.ck-autocomplete>.ck-search__results.ck-search__results_n {
    bottom: 100%;
    }

    .ck.ck-autocomplete>.ck-search__results.ck-search__results_s {
    bottom: auto;
    top: 100%;
    }

    .ck.ck-autocomplete>.ck-search__results {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-autocomplete>.ck-search__results,
    .ck.ck-autocomplete>.ck-search__results.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    }

    .ck.ck-autocomplete>.ck-search__results {
    background: var(--ck-color-base-background);
    border: 1px solid var(--ck-color-dropdown-panel-border);
    box-shadow: var(--ck-drop-shadow), 0 0;
    max-height: 200px;
    min-width: auto;
    overflow-y: auto;
    }

    .ck.ck-autocomplete>.ck-search__results.ck-search__results_n {
    border-bottom-left-radius: 0;
    border-bottom-right-radius: 0;
    margin-bottom: -1px;
    }

    .ck.ck-autocomplete>.ck-search__results.ck-search__results_s {
    border-top-left-radius: 0;
    border-top-right-radius: 0;
    margin-top: -1px;
    }

    .ck.ck-highlighted-text mark {
    background: var(--ck-color-highlight-background);
    font-size: inherit;
    font-weight: inherit;
    line-height: inherit;
    vertical-align: initial;
    }

    .ck.ck-collapsible.ck-collapsible_collapsed>.ck-collapsible__children {
    display: none;
    }

    :root {
    --ck-collapsible-arrow-size: calc(var(--ck-icon-size) * 0.5);
    }

    .ck.ck-collapsible>.ck.ck-button {
    border-radius: 0;
    color: inherit;
    font-weight: 700;
    padding: var(--ck-list-button-padding);
    width: 100%;
    }

    .ck.ck-collapsible>.ck.ck-button:focus {
    background: transparent;
    }

    .ck.ck-collapsible>.ck.ck-button:active,
    .ck.ck-collapsible>.ck.ck-button:hover:not(:focus),
    .ck.ck-collapsible>.ck.ck-button:not(:focus) {
    background: transparent;
    border-color: transparent;
    box-shadow: none;
    }

    .ck.ck-collapsible>.ck.ck-button>.ck-icon {
    margin-right: var(--ck-spacing-medium);
    width: var(--ck-collapsible-arrow-size);
    }

    .ck.ck-collapsible>.ck-collapsible__children {
    padding: var(--ck-spacing-medium) var(--ck-spacing-large) var(--ck-spacing-large);
    }

    .ck.ck-collapsible.ck-collapsible_collapsed>.ck.ck-button .ck-icon {
    transform: rotate(-90deg);
    }

    .ck.ck-spinner-container {
    display: block;
    position: relative;
    }

    .ck.ck-spinner {
    left: 0;
    margin: 0 auto;
    position: absolute;
    right: 0;
    top: 50%;
    transform: translateY(-50%);
    z-index: 1;
    }

    :root {
    --ck-toolbar-spinner-size: 18px;
    }

    .ck.ck-spinner-container {
    animation: rotate 1.5s linear infinite;
    }

    .ck.ck-spinner,
    .ck.ck-spinner-container {
    height: var(--ck-toolbar-spinner-size);
    width: var(--ck-toolbar-spinner-size);
    }

    .ck.ck-spinner {
    border: 2px solid var(--ck-color-text);
    border-radius: 50%;
    border-top: 2px solid transparent;
    }

    @keyframes rotate {
    to {
        transform: rotate(1turn);
    }
    }

    .ck.ck-block-toolbar-button {
    position: absolute;
    z-index: var(--ck-z-default);
    }

    :root {
    --ck-color-block-toolbar-button: var(--ck-color-text);
    --ck-block-toolbar-button-size: var(--ck-font-size-normal);
    }

    .ck.ck-block-toolbar-button {
    color: var(--ck-color-block-toolbar-button);
    font-size: var(--ck-block-toolbar-size);
    }

    .ck.ck-editor {
    position: relative;
    }

    .ck.ck-editor .ck-editor__top .ck-sticky-panel .ck-toolbar {
    z-index: var(--ck-z-modal);
    }

    .ck.ck-editor__top .ck-sticky-panel .ck-toolbar {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-editor__top .ck-sticky-panel .ck-toolbar,
    .ck.ck-editor__top .ck-sticky-panel .ck-toolbar.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    border-bottom-left-radius: 0;
    border-bottom-right-radius: 0;
    }

    .ck.ck-editor__top .ck-sticky-panel .ck-toolbar {
    border-bottom-width: 0;
    }

    .ck.ck-editor__top .ck-sticky-panel .ck-sticky-panel__content_sticky .ck-toolbar {
    border-bottom-width: 1px;
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-editor__top .ck-sticky-panel .ck-sticky-panel__content_sticky .ck-toolbar,
    .ck.ck-editor__top .ck-sticky-panel .ck-sticky-panel__content_sticky .ck-toolbar.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    border-radius: 0;
    }

    .ck.ck-editor__main>.ck-editor__editable {
    background: var(--ck-color-base-background);
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-editor__main>.ck-editor__editable,
    .ck.ck-editor__main>.ck-editor__editable.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    border-top-left-radius: 0;
    border-top-right-radius: 0;
    }

    .ck.ck-editor__main>.ck-editor__editable:not(.ck-focused) {
    border-color: var(--ck-color-base-border);
    }

    .ck-content code {
    background-color: hsla(0, 0%, 78%, 0.3);
    border-radius: 2px;
    padding: 0.15em;
    }

    .ck.ck-editor__editable .ck-code_selected {
    background-color: hsla(0, 0%, 78%, 0.5);
    }

    .ck-content blockquote {
    border-left: 5px solid #ccc;
    font-style: italic;
    margin-left: 0;
    margin-right: 0;
    overflow: hidden;
    padding-left: 1.5em;
    padding-right: 1.5em;
    }

    .ck-content[dir='rtl'] blockquote {
    border-left: 0;
    border-right: 5px solid #ccc;
    }

    .ck .ck-widget .ck-widget__type-around__button {
    display: block;
    overflow: hidden;
    position: absolute;
    z-index: var(--ck-z-default);
    }

    .ck .ck-widget .ck-widget__type-around__button svg {
    left: 50%;
    position: absolute;
    top: 50%;
    z-index: calc(var(--ck-z-default) + 2);
    }

    .ck .ck-widget .ck-widget__type-around__button.ck-widget__type-around__button_before {
    left: min(10%, 30px);
    top: calc(var(--ck-widget-outline-thickness) * -0.5);
    transform: translateY(-50%);
    }

    .ck .ck-widget .ck-widget__type-around__button.ck-widget__type-around__button_after {
    bottom: calc(var(--ck-widget-outline-thickness) * -0.5);
    right: min(10%, 30px);
    transform: translateY(50%);
    }

    .ck .ck-widget.ck-widget_selected>.ck-widget__type-around>.ck-widget__type-around__button:after,
    .ck .ck-widget>.ck-widget__type-around>.ck-widget__type-around__button:hover:after {
    content: '';
    display: block;
    left: 1px;
    position: absolute;
    top: 1px;
    z-index: calc(var(--ck-z-default) + 1);
    }

    .ck .ck-widget>.ck-widget__type-around>.ck-widget__type-around__fake-caret {
    display: none;
    left: 0;
    position: absolute;
    right: 0;
    }

    .ck .ck-widget:hover>.ck-widget__type-around>.ck-widget__type-around__fake-caret {
    left: calc(var(--ck-widget-outline-thickness) * -1);
    right: calc(var(--ck-widget-outline-thickness) * -1);
    }

    .ck .ck-widget.ck-widget_type-around_show-fake-caret_before>.ck-widget__type-around>.ck-widget__type-around__fake-caret {
    display: block;
    top: calc(var(--ck-widget-outline-thickness) * -1 - 1px);
    }

    .ck .ck-widget.ck-widget_type-around_show-fake-caret_after>.ck-widget__type-around>.ck-widget__type-around__fake-caret {
    bottom: calc(var(--ck-widget-outline-thickness) * -1 - 1px);
    display: block;
    }

    .ck.ck-editor__editable.ck-read-only .ck-widget__type-around,
    .ck.ck-editor__editable.ck-restricted-editing_mode_restricted .ck-widget__type-around,
    .ck.ck-editor__editable.ck-widget__type-around_disabled .ck-widget__type-around {
    display: none;
    }

    :root {
    --ck-widget-type-around-button-size: 20px;
    --ck-color-widget-type-around-button-active: var(--ck-color-focus-border);
    --ck-color-widget-type-around-button-hover: var(--ck-color-widget-hover-border);
    --ck-color-widget-type-around-button-blurred-editable: var(--ck-color-widget-blurred-border);
    --ck-color-widget-type-around-button-radar-start-alpha: 0;
    --ck-color-widget-type-around-button-radar-end-alpha: 0.3;
    --ck-color-widget-type-around-button-icon: var(--ck-color-base-background);
    }

    .ck .ck-widget .ck-widget__type-around__button {
    background: var(--ck-color-widget-type-around-button);
    border-radius: 100px;
    height: var(--ck-widget-type-around-button-size);
    opacity: 0;
    pointer-events: none;
    transition: opacity var(--ck-widget-handler-animation-duration) var(--ck-widget-handler-animation-curve),
        background var(--ck-widget-handler-animation-duration) var(--ck-widget-handler-animation-curve);
    width: var(--ck-widget-type-around-button-size);
    }

    .ck .ck-widget .ck-widget__type-around__button svg {
    height: 8px;
    margin-top: 1px;
    transform: translate(-50%, -50%);
    transition: transform 0.5s ease;
    width: 10px;
    }

    .ck .ck-widget .ck-widget__type-around__button svg * {
    stroke-dasharray: 10;
    stroke-dashoffset: 0;
    fill: none;
    stroke: var(--ck-color-widget-type-around-button-icon);
    stroke-width: 1.5px;
    stroke-linecap: round;
    stroke-linejoin: round;
    }

    .ck .ck-widget .ck-widget__type-around__button svg line {
    stroke-dasharray: 7;
    }

    .ck .ck-widget .ck-widget__type-around__button:hover {
    animation: ck-widget-type-around-button-sonar 1s ease infinite;
    }

    .ck .ck-widget .ck-widget__type-around__button:hover svg polyline {
    animation: ck-widget-type-around-arrow-dash 2s linear;
    }

    .ck .ck-widget .ck-widget__type-around__button:hover svg line {
    animation: ck-widget-type-around-arrow-tip-dash 2s linear;
    }

    .ck .ck-widget.ck-widget_selected>.ck-widget__type-around>.ck-widget__type-around__button,
    .ck .ck-widget:hover>.ck-widget__type-around>.ck-widget__type-around__button {
    opacity: 1;
    pointer-events: auto;
    }

    .ck .ck-widget:not(.ck-widget_selected)>.ck-widget__type-around>.ck-widget__type-around__button {
    background: var(--ck-color-widget-type-around-button-hover);
    }

    .ck .ck-widget.ck-widget_selected>.ck-widget__type-around>.ck-widget__type-around__button,
    .ck .ck-widget>.ck-widget__type-around>.ck-widget__type-around__button:hover {
    background: var(--ck-color-widget-type-around-button-active);
    }

    .ck .ck-widget.ck-widget_selected>.ck-widget__type-around>.ck-widget__type-around__button:after,
    .ck .ck-widget>.ck-widget__type-around>.ck-widget__type-around__button:hover:after {
    background: linear-gradient(135deg,
        hsla(0, 0%, 100%, 0),
        hsla(0, 0%, 100%, 0.3));
    border-radius: 100px;
    height: calc(var(--ck-widget-type-around-button-size) - 2px);
    width: calc(var(--ck-widget-type-around-button-size) - 2px);
    }

    .ck .ck-widget.ck-widget_with-selection-handle>.ck-widget__type-around>.ck-widget__type-around__button_before {
    margin-left: 20px;
    }

    .ck .ck-widget .ck-widget__type-around__fake-caret {
    animation: ck-widget-type-around-fake-caret-pulse 1s linear infinite normal forwards;
    background: var(--ck-color-base-text);
    height: 1px;
    outline: 1px solid hsla(0, 0%, 100%, 0.5);
    pointer-events: none;
    }

    .ck .ck-widget.ck-widget_selected.ck-widget_type-around_show-fake-caret_after,
    .ck .ck-widget.ck-widget_selected.ck-widget_type-around_show-fake-caret_before {
    outline-color: transparent;
    }

    .ck .ck-widget.ck-widget_type-around_show-fake-caret_after.ck-widget_selected:hover,
    .ck .ck-widget.ck-widget_type-around_show-fake-caret_before.ck-widget_selected:hover {
    outline-color: var(--ck-color-widget-hover-border);
    }

    .ck .ck-widget.ck-widget_type-around_show-fake-caret_after>.ck-widget__type-around>.ck-widget__type-around__button,
    .ck .ck-widget.ck-widget_type-around_show-fake-caret_before>.ck-widget__type-around>.ck-widget__type-around__button {
    opacity: 0;
    pointer-events: none;
    }

    .ck .ck-widget.ck-widget_type-around_show-fake-caret_after.ck-widget_selected.ck-widget_with-resizer>.ck-widget__resizer,
    .ck .ck-widget.ck-widget_type-around_show-fake-caret_after.ck-widget_with-selection-handle.ck-widget_selected:hover>.ck-widget__selection-handle,
    .ck .ck-widget.ck-widget_type-around_show-fake-caret_after.ck-widget_with-selection-handle.ck-widget_selected>.ck-widget__selection-handle,
    .ck .ck-widget.ck-widget_type-around_show-fake-caret_before.ck-widget_selected.ck-widget_with-resizer>.ck-widget__resizer,
    .ck .ck-widget.ck-widget_type-around_show-fake-caret_before.ck-widget_with-selection-handle.ck-widget_selected:hover>.ck-widget__selection-handle,
    .ck .ck-widget.ck-widget_type-around_show-fake-caret_before.ck-widget_with-selection-handle.ck-widget_selected>.ck-widget__selection-handle {
    opacity: 0;
    }

    .ck[dir='rtl'] .ck-widget.ck-widget_with-selection-handle .ck-widget__type-around>.ck-widget__type-around__button_before {
    margin-left: 0;
    margin-right: 20px;
    }

    .ck-editor__nested-editable.ck-editor__editable_selected .ck-widget.ck-widget_selected>.ck-widget__type-around>.ck-widget__type-around__button,
    .ck-editor__nested-editable.ck-editor__editable_selected .ck-widget:hover>.ck-widget__type-around>.ck-widget__type-around__button {
    opacity: 0;
    pointer-events: none;
    }

    .ck-editor__editable.ck-blurred .ck-widget.ck-widget_selected>.ck-widget__type-around>.ck-widget__type-around__button:not(:hover) {
    background: var(--ck-color-widget-type-around-button-blurred-editable);
    }

    .ck-editor__editable.ck-blurred .ck-widget.ck-widget_selected>.ck-widget__type-around>.ck-widget__type-around__button:not(:hover) svg * {
    stroke: #999;
    }

    @keyframes ck-widget-type-around-arrow-dash {
    0% {
        stroke-dashoffset: 10;
    }

    20%,
    to {
        stroke-dashoffset: 0;
    }
    }

    @keyframes ck-widget-type-around-arrow-tip-dash {

    0%,
    20% {
        stroke-dashoffset: 7;
    }

    40%,
    to {
        stroke-dashoffset: 0;
    }
    }

    @keyframes ck-widget-type-around-button-sonar {
    0% {
        box-shadow: 0 0 0 0 hsla(var(--ck-color-focus-border-coordinates),
            var(--ck-color-widget-type-around-button-radar-start-alpha));
    }

    50% {
        box-shadow: 0 0 0 5px hsla(var(--ck-color-focus-border-coordinates),
            var(--ck-color-widget-type-around-button-radar-end-alpha));
    }

    to {
        box-shadow: 0 0 0 5px hsla(var(--ck-color-focus-border-coordinates),
            var(--ck-color-widget-type-around-button-radar-start-alpha));
    }
    }

    @keyframes ck-widget-type-around-fake-caret-pulse {
    0% {
        opacity: 1;
    }

    49% {
        opacity: 1;
    }

    50% {
        opacity: 0;
    }

    99% {
        opacity: 0;
    }

    to {
        opacity: 1;
    }
    }

    :root {
    --ck-color-resizer: var(--ck-color-focus-border);
    --ck-color-resizer-tooltip-background: #262626;
    --ck-color-resizer-tooltip-text: #f2f2f2;
    --ck-resizer-border-radius: var(--ck-border-radius);
    --ck-resizer-tooltip-offset: 10px;
    --ck-resizer-tooltip-height: calc(var(--ck-spacing-small) * 2 + 10px);
    }

    .ck .ck-widget,
    .ck .ck-widget.ck-widget_with-selection-handle {
    position: relative;
    }

    .ck .ck-widget.ck-widget_with-selection-handle .ck-widget__selection-handle {
    position: absolute;
    }

    .ck .ck-widget.ck-widget_with-selection-handle .ck-widget__selection-handle .ck-icon {
    display: block;
    }

    .ck .ck-widget.ck-widget_with-selection-handle.ck-widget_selected>.ck-widget__selection-handle,
    .ck .ck-widget.ck-widget_with-selection-handle:hover>.ck-widget__selection-handle {
    visibility: visible;
    }

    .ck .ck-size-view {
    background: var(--ck-color-resizer-tooltip-background);
    border: 1px solid var(--ck-color-resizer-tooltip-text);
    border-radius: var(--ck-resizer-border-radius);
    color: var(--ck-color-resizer-tooltip-text);
    display: block;
    font-size: var(--ck-font-size-tiny);
    height: var(--ck-resizer-tooltip-height);
    line-height: var(--ck-resizer-tooltip-height);
    padding: 0 var(--ck-spacing-small);
    }

    .ck .ck-size-view.ck-orientation-above-center,
    .ck .ck-size-view.ck-orientation-bottom-left,
    .ck .ck-size-view.ck-orientation-bottom-right,
    .ck .ck-size-view.ck-orientation-top-left,
    .ck .ck-size-view.ck-orientation-top-right {
    position: absolute;
    }

    .ck .ck-size-view.ck-orientation-top-left {
    left: var(--ck-resizer-tooltip-offset);
    top: var(--ck-resizer-tooltip-offset);
    }

    .ck .ck-size-view.ck-orientation-top-right {
    right: var(--ck-resizer-tooltip-offset);
    top: var(--ck-resizer-tooltip-offset);
    }

    .ck .ck-size-view.ck-orientation-bottom-right {
    bottom: var(--ck-resizer-tooltip-offset);
    right: var(--ck-resizer-tooltip-offset);
    }

    .ck .ck-size-view.ck-orientation-bottom-left {
    bottom: var(--ck-resizer-tooltip-offset);
    left: var(--ck-resizer-tooltip-offset);
    }

    .ck .ck-size-view.ck-orientation-above-center {
    left: 50%;
    top: calc(var(--ck-resizer-tooltip-height) * -1);
    transform: translate(-50%);
    }

    :root {
    --ck-widget-outline-thickness: 3px;
    --ck-widget-handler-icon-size: 16px;
    --ck-widget-handler-animation-duration: 200ms;
    --ck-widget-handler-animation-curve: ease;
    --ck-color-widget-blurred-border: #dedede;
    --ck-color-widget-hover-border: #ffc83d;
    --ck-color-widget-editable-focus-background: var(--ck-color-base-background);
    --ck-color-widget-drag-handler-icon-color: var(--ck-color-base-background);
    }

    .ck .ck-widget {
    outline-color: transparent;
    outline-style: solid;
    outline-width: var(--ck-widget-outline-thickness);
    transition: outline-color var(--ck-widget-handler-animation-duration) var(--ck-widget-handler-animation-curve);
    }

    .ck .ck-widget.ck-widget_selected,
    .ck .ck-widget.ck-widget_selected:hover {
    outline: var(--ck-widget-outline-thickness) solid var(--ck-color-focus-border);
    }

    .ck .ck-widget:hover {
    outline-color: var(--ck-color-widget-hover-border);
    }

    .ck .ck-editor__nested-editable {
    border: 1px solid transparent;
    }

    .ck .ck-editor__nested-editable.ck-editor__nested-editable_focused,
    .ck .ck-editor__nested-editable:focus {
    background-color: var(--ck-color-widget-editable-focus-background);
    border: var(--ck-focus-ring);
    box-shadow: var(--ck-inner-shadow), 0 0;
    outline: none;
    }

    .ck .ck-widget.ck-widget_with-selection-handle .ck-widget__selection-handle {
    background-color: transparent;
    border-radius: var(--ck-border-radius) var(--ck-border-radius) 0 0;
    box-sizing: border-box;
    left: calc(0px - var(--ck-widget-outline-thickness));
    opacity: 0;
    padding: 4px;
    top: 0;
    transform: translateY(-100%);
    transition: background-color var(--ck-widget-handler-animation-duration) var(--ck-widget-handler-animation-curve),
        visibility var(--ck-widget-handler-animation-duration) var(--ck-widget-handler-animation-curve),
        opacity var(--ck-widget-handler-animation-duration) var(--ck-widget-handler-animation-curve);
    }

    .ck .ck-widget.ck-widget_with-selection-handle .ck-widget__selection-handle .ck-icon {
    color: var(--ck-color-widget-drag-handler-icon-color);
    height: var(--ck-widget-handler-icon-size);
    width: var(--ck-widget-handler-icon-size);
    }

    .ck .ck-widget.ck-widget_with-selection-handle .ck-widget__selection-handle .ck-icon .ck-icon__selected-indicator {
    opacity: 0;
    transition: opacity 0.3s var(--ck-widget-handler-animation-curve);
    }

    .ck .ck-widget.ck-widget_with-selection-handle .ck-widget__selection-handle:hover .ck-icon .ck-icon__selected-indicator {
    opacity: 1;
    }

    .ck .ck-widget.ck-widget_with-selection-handle:hover>.ck-widget__selection-handle {
    background-color: var(--ck-color-widget-hover-border);
    opacity: 1;
    }

    .ck .ck-widget.ck-widget_with-selection-handle.ck-widget_selected:hover>.ck-widget__selection-handle,
    .ck .ck-widget.ck-widget_with-selection-handle.ck-widget_selected>.ck-widget__selection-handle {
    background-color: var(--ck-color-focus-border);
    opacity: 1;
    }

    .ck .ck-widget.ck-widget_with-selection-handle.ck-widget_selected:hover>.ck-widget__selection-handle .ck-icon .ck-icon__selected-indicator,
    .ck .ck-widget.ck-widget_with-selection-handle.ck-widget_selected>.ck-widget__selection-handle .ck-icon .ck-icon__selected-indicator {
    opacity: 1;
    }

    .ck[dir='rtl'] .ck-widget.ck-widget_with-selection-handle .ck-widget__selection-handle {
    left: auto;
    right: calc(0px - var(--ck-widget-outline-thickness));
    }

    .ck.ck-editor__editable.ck-read-only .ck-widget {
    transition: none;
    }

    .ck.ck-editor__editable.ck-read-only .ck-widget:not(.ck-widget_selected) {
    --ck-widget-outline-thickness: 0px;
    }

    .ck.ck-editor__editable.ck-read-only .ck-widget.ck-widget_with-selection-handle .ck-widget__selection-handle,
    .ck.ck-editor__editable.ck-read-only .ck-widget.ck-widget_with-selection-handle .ck-widget__selection-handle:hover {
    background: var(--ck-color-widget-blurred-border);
    }

    .ck.ck-editor__editable.ck-blurred .ck-widget.ck-widget_selected,
    .ck.ck-editor__editable.ck-blurred .ck-widget.ck-widget_selected:hover {
    outline-color: var(--ck-color-widget-blurred-border);
    }

    .ck.ck-editor__editable.ck-blurred .ck-widget.ck-widget_selected.ck-widget_with-selection-handle:hover>.ck-widget__selection-handle,
    .ck.ck-editor__editable.ck-blurred .ck-widget.ck-widget_selected.ck-widget_with-selection-handle:hover>.ck-widget__selection-handle:hover,
    .ck.ck-editor__editable.ck-blurred .ck-widget.ck-widget_selected.ck-widget_with-selection-handle>.ck-widget__selection-handle,
    .ck.ck-editor__editable.ck-blurred .ck-widget.ck-widget_selected.ck-widget_with-selection-handle>.ck-widget__selection-handle:hover {
    background: var(--ck-color-widget-blurred-border);
    }

    .ck.ck-editor__editable blockquote>.ck-widget.ck-widget_with-selection-handle:first-child,
    .ck.ck-editor__editable>.ck-widget.ck-widget_with-selection-handle:first-child {
    margin-top: calc(1em + var(--ck-widget-handler-icon-size));
    }

    .ck .ck-widget_with-resizer {
    position: relative;
    }

    .ck .ck-widget__resizer {
    display: none;
    left: 0;
    pointer-events: none;
    position: absolute;
    top: 0;
    }

    .ck-focused .ck-widget_with-resizer.ck-widget_selected>.ck-widget__resizer {
    display: block;
    }

    .ck .ck-widget__resizer__handle {
    pointer-events: all;
    position: absolute;
    }

    .ck .ck-widget__resizer__handle.ck-widget__resizer__handle-bottom-right,
    .ck .ck-widget__resizer__handle.ck-widget__resizer__handle-top-left {
    cursor: nwse-resize;
    }

    .ck .ck-widget__resizer__handle.ck-widget__resizer__handle-bottom-left,
    .ck .ck-widget__resizer__handle.ck-widget__resizer__handle-top-right {
    cursor: nesw-resize;
    }

    :root {
    --ck-resizer-size: 10px;
    --ck-resizer-offset: calc(var(--ck-resizer-size) / -2 - 2px);
    --ck-resizer-border-width: 1px;
    }

    .ck .ck-widget__resizer {
    outline: 1px solid var(--ck-color-resizer);
    }

    .ck .ck-widget__resizer__handle {
    background: var(--ck-color-focus-border);
    border: var(--ck-resizer-border-width) solid #fff;
    border-radius: var(--ck-resizer-border-radius);
    height: var(--ck-resizer-size);
    width: var(--ck-resizer-size);
    }

    .ck .ck-widget__resizer__handle.ck-widget__resizer__handle-top-left {
    left: var(--ck-resizer-offset);
    top: var(--ck-resizer-offset);
    }

    .ck .ck-widget__resizer__handle.ck-widget__resizer__handle-top-right {
    right: var(--ck-resizer-offset);
    top: var(--ck-resizer-offset);
    }

    .ck .ck-widget__resizer__handle.ck-widget__resizer__handle-bottom-right {
    bottom: var(--ck-resizer-offset);
    right: var(--ck-resizer-offset);
    }

    .ck .ck-widget__resizer__handle.ck-widget__resizer__handle-bottom-left {
    bottom: var(--ck-resizer-offset);
    left: var(--ck-resizer-offset);
    }

    .ck.ck-editor__editable .ck.ck-clipboard-drop-target-position {
    display: inline;
    pointer-events: none;
    position: relative;
    }

    .ck.ck-editor__editable .ck.ck-clipboard-drop-target-position span {
    position: absolute;
    width: 0;
    }

    .ck.ck-editor__editable .ck-widget:-webkit-drag>.ck-widget__selection-handle,
    .ck.ck-editor__editable .ck-widget:-webkit-drag>.ck-widget__type-around {
    display: none;
    }

    .ck.ck-clipboard-drop-target-line {
    pointer-events: none;
    position: absolute;
    }

    :root {
    --ck-clipboard-drop-target-dot-width: 12px;
    --ck-clipboard-drop-target-dot-height: 8px;
    --ck-clipboard-drop-target-color: var(--ck-color-focus-border);
    }

    .ck.ck-editor__editable .ck.ck-clipboard-drop-target-position span {
    background: var(--ck-clipboard-drop-target-color);
    border: 1px solid var(--ck-clipboard-drop-target-color);
    bottom: calc(var(--ck-clipboard-drop-target-dot-height) * -0.5);
    margin-left: -1px;
    top: calc(var(--ck-clipboard-drop-target-dot-height) * -0.5);
    }

    .ck.ck-editor__editable .ck.ck-clipboard-drop-target-position span:after {
    border-color: var(--ck-clipboard-drop-target-color) transparent transparent transparent;
    border-style: solid;
    border-width: calc(var(--ck-clipboard-drop-target-dot-height)) calc(var(--ck-clipboard-drop-target-dot-width) * 0.5) 0 calc(var(--ck-clipboard-drop-target-dot-width) * 0.5);
    content: '';
    display: block;
    height: 0;
    left: 50%;
    position: absolute;
    top: calc(var(--ck-clipboard-drop-target-dot-height) * -0.5);
    transform: translateX(-50%);
    width: 0;
    }

    .ck.ck-editor__editable .ck-widget.ck-clipboard-drop-target-range {
    outline: var(--ck-widget-outline-thickness) solid var(--ck-clipboard-drop-target-color) !important;
    }

    .ck.ck-editor__editable .ck-widget:-webkit-drag {
    zoom: 0.6;
    outline: none !important;
    }

    .ck.ck-clipboard-drop-target-line {
    background: var(--ck-clipboard-drop-target-color);
    border: 1px solid var(--ck-clipboard-drop-target-color);
    height: 0;
    margin-top: -1px;
    }

    .ck.ck-clipboard-drop-target-line:before {
    border-style: solid;
    content: '';
    height: 0;
    position: absolute;
    top: calc(var(--ck-clipboard-drop-target-dot-width) * -0.5);
    width: 0;
    }

    [dir='ltr'] .ck.ck-clipboard-drop-target-line:before {
    border-color: transparent transparent transparent var(--ck-clipboard-drop-target-color);
    border-width: calc(var(--ck-clipboard-drop-target-dot-width) * 0.5) 0 calc(var(--ck-clipboard-drop-target-dot-width) * 0.5) var(--ck-clipboard-drop-target-dot-height);
    left: -1px;
    }

    [dir='rtl'] .ck.ck-clipboard-drop-target-line:before {
    border-color: transparent var(--ck-clipboard-drop-target-color) transparent transparent;
    border-width: calc(var(--ck-clipboard-drop-target-dot-width) * 0.5) var(--ck-clipboard-drop-target-dot-height) calc(var(--ck-clipboard-drop-target-dot-width) * 0.5) 0;
    right: -1px;
    }

    .ck-vertical-form .ck-button:after {
    bottom: -1px;
    content: '';
    position: absolute;
    right: -1px;
    top: -1px;
    width: 0;
    z-index: 1;
    }

    .ck-vertical-form .ck-button:focus:after {
    display: none;
    }

    @media screen and (max-width: 600px) {
    .ck.ck-responsive-form .ck-button:after {
        bottom: -1px;
        content: '';
        position: absolute;
        right: -1px;
        top: -1px;
        width: 0;
        z-index: 1;
    }

    .ck.ck-responsive-form .ck-button:focus:after {
        display: none;
    }
    }

    .ck-vertical-form>.ck-button:nth-last-child(2):after {
    border-right: 1px solid var(--ck-color-base-border);
    }

    .ck.ck-responsive-form {
    padding: var(--ck-spacing-large);
    }

    .ck.ck-responsive-form:focus {
    outline: none;
    }

    [dir='ltr'] .ck.ck-responsive-form> :not(:first-child),
    [dir='rtl'] .ck.ck-responsive-form> :not(:last-child) {
    margin-left: var(--ck-spacing-standard);
    }

    @media screen and (max-width: 600px) {
    .ck.ck-responsive-form {
        padding: 0;
        width: calc(var(--ck-input-width) * 0.8);
    }

    .ck.ck-responsive-form .ck-labeled-field-view {
        margin: var(--ck-spacing-large) var(--ck-spacing-large) 0;
    }

    .ck.ck-responsive-form .ck-labeled-field-view .ck-input-text {
        min-width: 0;
        width: 100%;
    }

    .ck.ck-responsive-form .ck-labeled-field-view .ck-labeled-field-view__error {
        white-space: normal;
    }

    .ck.ck-responsive-form>.ck-button:nth-last-child(2):after {
        border-right: 1px solid var(--ck-color-base-border);
    }

    .ck.ck-responsive-form>.ck-button:last-child,
    .ck.ck-responsive-form>.ck-button:nth-last-child(2) {
        border-radius: 0;
        margin-top: var(--ck-spacing-large);
        padding: var(--ck-spacing-standard);
    }

    .ck.ck-responsive-form>.ck-button:last-child:not(:focus),
    .ck.ck-responsive-form>.ck-button:nth-last-child(2):not(:focus) {
        border-top: 1px solid var(--ck-color-base-border);
    }

    [dir='ltr'] .ck.ck-responsive-form>.ck-button:last-child,
    [dir='ltr'] .ck.ck-responsive-form>.ck-button:nth-last-child(2),
    [dir='rtl'] .ck.ck-responsive-form>.ck-button:last-child,
    [dir='rtl'] .ck.ck-responsive-form>.ck-button:nth-last-child(2) {
        margin-left: 0;
    }

    [dir='rtl'] .ck.ck-responsive-form>.ck-button:last-child:last-of-type,
    [dir='rtl'] .ck.ck-responsive-form>.ck-button:nth-last-child(2):last-of-type {
        border-right: 1px solid var(--ck-color-base-border);
    }
    }

    .ck.ck-find-and-replace-form {
    max-width: 100%;
    }

    .ck.ck-find-and-replace-form fieldset {
    display: flex;
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find .ck-results-counter {
    position: absolute;
    }

    .ck.ck-find-and-replace-form {
    width: 400px;
    }

    .ck.ck-find-and-replace-form:focus {
    outline: none;
    }

    .ck.ck-find-and-replace-form fieldset {
    align-content: stretch;
    align-items: center;
    border: 0;
    flex-direction: row;
    flex-wrap: nowrap;
    margin: 0;
    padding: var(--ck-spacing-large);
    }

    .ck.ck-find-and-replace-form fieldset>.ck-button {
    flex: 0 0 auto;
    }

    [dir='ltr'] .ck.ck-find-and-replace-form fieldset>*+* {
    margin-left: var(--ck-spacing-standard);
    }

    [dir='rtl'] .ck.ck-find-and-replace-form fieldset>*+* {
    margin-right: var(--ck-spacing-standard);
    }

    .ck.ck-find-and-replace-form fieldset .ck-labeled-field-view {
    flex: 1 1 auto;
    }

    .ck.ck-find-and-replace-form fieldset .ck-labeled-field-view .ck-input {
    min-width: 50px;
    width: 100%;
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find {
    align-items: flex-start;
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find>.ck-button-find {
    font-weight: 700;
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find>.ck-button-find .ck-button__label {
    padding-left: var(--ck-spacing-large);
    padding-right: var(--ck-spacing-large);
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find>.ck-button-prev>.ck-icon {
    transform: rotate(90deg);
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find>.ck-button-next>.ck-icon {
    transform: rotate(-90deg);
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find .ck-results-counter {
    top: 50%;
    transform: translateY(-50%);
    }

    [dir='ltr'] .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find .ck-results-counter {
    right: var(--ck-spacing-standard);
    }

    [dir='rtl'] .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find .ck-results-counter {
    left: var(--ck-spacing-standard);
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find .ck-results-counter {
    color: var(--ck-color-base-border);
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__replace {
    flex-wrap: wrap;
    justify-content: flex-end;
    margin-top: calc(var(--ck-spacing-large) * -1);
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__replace>.ck-labeled-field-view {
    margin-bottom: var(--ck-spacing-large);
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__replace>.ck-options-dropdown {
    margin-left: 0;
    margin-right: auto;
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__replace>.ck-labeled-field-view,
    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__replace>.ck-labeled-field-view .ck-input {
    width: 100%;
    }

    @media screen and (max-width: 600px) {
    .ck.ck-find-and-replace-form {
        width: 300px;
    }

    .ck.ck-find-and-replace-form fieldset {
        flex-wrap: wrap;
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find .ck-labeled-field-view {
        flex: 1 0 auto;
        margin-bottom: var(--ck-spacing-standard);
        width: 100%;
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find>.ck-button {
        text-align: center;
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find>.ck-button:first-of-type {
        flex: 1 1 auto;
    }

    [dir='ltr'] .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find>.ck-button:first-of-type {
        margin-left: 0;
    }

    [dir='rtl'] .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find>.ck-button:first-of-type {
        margin-right: 0;
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__find>.ck-button:first-of-type .ck-button__label {
        text-align: center;
        width: 100%;
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__replace> :not(.ck-labeled-field-view) {
        flex: 1 1 auto;
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__replace>.ck-dropdown:not(.ck-labeled-field-view) {
        flex-grow: 0;
    }

    .ck.ck-find-and-replace-form fieldset.ck-find-and-replace-form__replace>.ck-button:not(.ck-labeled-field-view)>.ck-button__label {
        text-align: center;
        width: 100%;
    }
    }

    .ck-find-result {
    background: var(--ck-color-highlight-background);
    color: var(--ck-color-text);
    }

    .ck-find-result_selected {
    background: #ff9633;
    }

    .ck-content .text-tiny {
    font-size: 0.7em;
    }

    .ck-content .text-small {
    font-size: 0.85em;
    }

    .ck-content .text-big {
    font-size: 1.4em;
    }

    .ck-content .text-huge {
    font-size: 1.8em;
    }

    .ck.ck-heading_heading1 {
    font-size: 20px;
    }

    .ck.ck-heading_heading2 {
    font-size: 17px;
    }

    .ck.ck-heading_heading3 {
    font-size: 14px;
    }

    .ck[class*='ck-heading_heading'] {
    font-weight: 700;
    }

    .ck.ck-dropdown.ck-heading-dropdown .ck-dropdown__button .ck-button__label {
    width: 8em;
    }

    .ck.ck-dropdown.ck-heading-dropdown .ck-dropdown__panel .ck-list__item {
    min-width: 18em;
    }

    .ck-editor__editable .ck-horizontal-line {
    display: flow-root;
    }

    .ck-content hr {
    background: #dedede;
    border: 0;
    height: 4px;
    margin: 15px 0;
    }

    .ck.ck-text-alternative-form {
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    }

    .ck.ck-text-alternative-form .ck-labeled-field-view {
    display: inline-block;
    }

    .ck.ck-text-alternative-form .ck-label {
    display: none;
    }

    @media screen and (max-width: 600px) {
    .ck.ck-text-alternative-form {
        flex-wrap: wrap;
    }

    .ck.ck-text-alternative-form .ck-labeled-field-view {
        flex-basis: 100%;
    }

    .ck.ck-text-alternative-form .ck-button {
        flex-basis: 50%;
    }
    }

    .ck.ck-editor__editable img.image_placeholder {
    background-size: 100% 100%;
    }

    .ck.ck-image-insert-url .ck-image-insert-url__action-row {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    }

    :root {
    --ck-image-insert-insert-by-url-width: 250px;
    }

    .ck.ck-image-insert-url {
    --ck-input-width: 100%;
    }

    .ck.ck-image-insert-url .ck-image-insert-url__action-row {
    grid-column-gap: var(--ck-spacing-large);
    margin-top: var(--ck-spacing-large);
    }

    .ck.ck-image-insert-url .ck-image-insert-url__action-row .ck-button-cancel,
    .ck.ck-image-insert-url .ck-image-insert-url__action-row .ck-button-save {
    justify-content: center;
    min-width: auto;
    }

    .ck.ck-image-insert-url .ck-image-insert-url__action-row .ck-button .ck-button__label {
    color: var(--ck-color-text);
    }

    .ck.ck-image-insert-form>.ck.ck-button {
    display: block;
    padding: var(--ck-list-button-padding);
    width: 100%;
    }

    [dir='ltr'] .ck.ck-image-insert-form>.ck.ck-button {
    text-align: left;
    }

    [dir='rtl'] .ck.ck-image-insert-form>.ck.ck-button {
    text-align: right;
    }

    .ck.ck-image-insert-form>.ck.ck-collapsible:not(:first-child) {
    border-top: 1px solid var(--ck-color-base-border);
    }

    .ck.ck-image-insert-form>.ck.ck-collapsible:not(:last-child) {
    border-bottom: 1px solid var(--ck-color-base-border);
    }

    .ck.ck-image-insert-form>.ck.ck-collapsible,
    .ck.ck-image-insert-form>.ck.ck-image-insert-url {
    min-width: var(--ck-image-insert-insert-by-url-width);
    }

    .ck.ck-image-insert-form>.ck.ck-image-insert-url {
    padding: var(--ck-spacing-large);
    }

    .ck.ck-image-insert-form:focus {
    outline: none;
    }

    .ck-content .image {
    clear: both;
    display: table;
    margin: 0.9em auto;
    min-width: 50px;
    text-align: center;
    }

    .ck-content .image img {
    display: block;
    height: auto;
    margin: 0 auto;
    max-width: 100%;
    min-width: 100%;
    }

    .ck-content .image-inline {
    align-items: flex-start;
    display: inline-flex;
    max-width: 100%;
    }

    .ck-content .image-inline picture {
    display: flex;
    }

    .ck-content .image-inline img,
    .ck-content .image-inline picture {
    flex-grow: 1;
    flex-shrink: 1;
    max-width: 100%;
    }

    .ck.ck-editor__editable .image>figcaption.ck-placeholder:before {
    overflow: hidden;
    padding-left: inherit;
    padding-right: inherit;
    text-overflow: ellipsis;
    white-space: nowrap;
    }

    .ck.ck-editor__editable .image {
    z-index: 1;
    }

    .ck.ck-editor__editable .image.ck-widget_selected {
    z-index: 2;
    }

    .ck.ck-editor__editable .image-inline {
    z-index: 1;
    }

    .ck.ck-editor__editable .image-inline.ck-widget_selected {
    z-index: 2;
    }

    .ck.ck-editor__editable .image-inline.ck-widget_selected ::selection {
    display: none;
    }

    .ck.ck-editor__editable .image-inline img {
    height: auto;
    }

    .ck.ck-editor__editable td .image-inline img,
    .ck.ck-editor__editable th .image-inline img {
    max-width: none;
    }

    :root {
    --ck-color-image-caption-background: #f7f7f7;
    --ck-color-image-caption-text: #333;
    --ck-color-image-caption-highligted-background: #fd0;
    }

    .ck-content .image>figcaption {
    background-color: var(--ck-color-image-caption-background);
    caption-side: bottom;
    color: var(--ck-color-image-caption-text);
    display: table-caption;
    font-size: 0.75em;
    outline-offset: -1px;
    padding: 0.6em;
    word-break: break-word;
    }

    .ck.ck-editor__editable .image>figcaption.image__caption_highlighted {
    animation: ck-image-caption-highlight 0.6s ease-out;
    }

    @keyframes ck-image-caption-highlight {
    0% {
        background-color: var(--ck-color-image-caption-highligted-background);
    }

    to {
        background-color: var(--ck-color-image-caption-background);
    }
    }

    .ck.ck-editor__editable .image,
    .ck.ck-editor__editable .image-inline {
    position: relative;
    }

    .ck.ck-editor__editable .image .ck-progress-bar,
    .ck.ck-editor__editable .image-inline .ck-progress-bar {
    left: 0;
    position: absolute;
    top: 0;
    }

    .ck.ck-editor__editable .image-inline.ck-appear,
    .ck.ck-editor__editable .image.ck-appear {
    animation: fadeIn 0.7s;
    }

    .ck.ck-editor__editable .image .ck-progress-bar,
    .ck.ck-editor__editable .image-inline .ck-progress-bar {
    background: var(--ck-color-upload-bar-background);
    height: 2px;
    transition: width 0.1s;
    width: 0;
    }

    @keyframes fadeIn {
    0% {
        opacity: 0;
    }

    to {
        opacity: 1;
    }
    }

    .ck-image-upload-complete-icon {
    border-radius: 50%;
    display: block;
    position: absolute;
    right: min(var(--ck-spacing-medium), 6%);
    top: min(var(--ck-spacing-medium), 6%);
    z-index: 1;
    }

    .ck-image-upload-complete-icon:after {
    content: '';
    position: absolute;
    }

    :root {
    --ck-color-image-upload-icon: #fff;
    --ck-color-image-upload-icon-background: #008a00;
    --ck-image-upload-icon-size: 20;
    --ck-image-upload-icon-width: 2px;
    --ck-image-upload-icon-is-visible: clamp(0px, 100% - 50px, 1px);
    }

    .ck-image-upload-complete-icon {
    animation-delay: 0ms, 3s;
    animation-duration: 0.5s, 0.5s;
    animation-fill-mode: forwards, forwards;
    animation-name: ck-upload-complete-icon-show, ck-upload-complete-icon-hide;
    background: var(--ck-color-image-upload-icon-background);
    font-size: calc(1px * var(--ck-image-upload-icon-size));
    height: calc(var(--ck-image-upload-icon-is-visible) * var(--ck-image-upload-icon-size));
    opacity: 0;
    overflow: hidden;
    width: calc(var(--ck-image-upload-icon-is-visible) * var(--ck-image-upload-icon-size));
    }

    .ck-image-upload-complete-icon:after {
    animation-delay: 0.5s;
    animation-duration: 0.5s;
    animation-fill-mode: forwards;
    animation-name: ck-upload-complete-icon-check;
    border-right: var(--ck-image-upload-icon-width) solid var(--ck-color-image-upload-icon);
    border-top: var(--ck-image-upload-icon-width) solid var(--ck-color-image-upload-icon);
    box-sizing: border-box;
    height: 0;
    left: 25%;
    opacity: 0;
    top: 50%;
    transform: scaleX(-1) rotate(135deg);
    transform-origin: left top;
    width: 0;
    }

    @keyframes ck-upload-complete-icon-show {
    0% {
        opacity: 0;
    }

    to {
        opacity: 1;
    }
    }

    @keyframes ck-upload-complete-icon-hide {
    0% {
        opacity: 1;
    }

    to {
        opacity: 0;
    }
    }

    @keyframes ck-upload-complete-icon-check {
    0% {
        height: 0;
        opacity: 1;
        width: 0;
    }

    33% {
        height: 0;
        width: 0.3em;
    }

    to {
        height: 0.45em;
        opacity: 1;
        width: 0.3em;
    }
    }

    .ck .ck-upload-placeholder-loader {
    align-items: center;
    display: flex;
    justify-content: center;
    left: 0;
    position: absolute;
    top: 0;
    }

    .ck .ck-upload-placeholder-loader:before {
    content: '';
    position: relative;
    }

    :root {
    --ck-color-upload-placeholder-loader: #b3b3b3;
    --ck-upload-placeholder-loader-size: 32px;
    --ck-upload-placeholder-image-aspect-ratio: 2.8;
    }

    .ck .ck-image-upload-placeholder {
    margin: 0;
    width: 100%;
    }

    .ck .ck-image-upload-placeholder.image-inline {
    width: calc(var(--ck-upload-placeholder-loader-size) * 2 * var(--ck-upload-placeholder-image-aspect-ratio));
    }

    .ck .ck-image-upload-placeholder img {
    aspect-ratio: var(--ck-upload-placeholder-image-aspect-ratio);
    }

    .ck .ck-upload-placeholder-loader {
    height: 100%;
    width: 100%;
    }

    .ck .ck-upload-placeholder-loader:before {
    animation: ck-upload-placeholder-loader 1s linear infinite;
    border-radius: 50%;
    border-right: 2px solid transparent;
    border-top: 3px solid var(--ck-color-upload-placeholder-loader);
    height: var(--ck-upload-placeholder-loader-size);
    width: var(--ck-upload-placeholder-loader-size);
    }

    @keyframes ck-upload-placeholder-loader {
    to {
        transform: rotate(1turn);
    }
    }

    .ck-content img.image_resized {
    height: auto;
    }

    .ck-content .image.image_resized {
    box-sizing: border-box;
    display: block;
    max-width: 100%;
    }

    .ck-content .image.image_resized img {
    width: 100%;
    }

    .ck-content .image.image_resized>figcaption {
    display: block;
    }

    .ck.ck-editor__editable td .image-inline.image_resized img,
    .ck.ck-editor__editable th .image-inline.image_resized img {
    max-width: 100%;
    }

    [dir='ltr'] .ck.ck-button.ck-button_with-text.ck-resize-image-button .ck-button__icon {
    margin-right: var(--ck-spacing-standard);
    }

    [dir='rtl'] .ck.ck-button.ck-button_with-text.ck-resize-image-button .ck-button__icon {
    margin-left: var(--ck-spacing-standard);
    }

    .ck.ck-dropdown .ck-button.ck-resize-image-button .ck-button__label {
    width: 4em;
    }

    :root {
    --ck-image-style-spacing: 1.5em;
    --ck-inline-image-style-spacing: calc(var(--ck-image-style-spacing) / 2);
    }

    .ck-content .image-style-block-align-left,
    .ck-content .image-style-block-align-right {
    max-width: calc(100% - var(--ck-image-style-spacing));
    }

    .ck-content .image-style-align-left,
    .ck-content .image-style-align-right {
    clear: none;
    }

    .ck-content .image-style-side {
    float: right;
    margin-left: var(--ck-image-style-spacing);
    max-width: 50%;
    }

    .ck-content .image-style-align-left {
    float: left;
    margin-right: var(--ck-image-style-spacing);
    }

    .ck-content .image-style-align-center {
    margin-left: auto;
    margin-right: auto;
    }

    .ck-content .image-style-align-right {
    float: right;
    margin-left: var(--ck-image-style-spacing);
    }

    .ck-content .image-style-block-align-right {
    margin-left: auto;
    margin-right: 0;
    }

    .ck-content .image-style-block-align-left {
    margin-left: 0;
    margin-right: auto;
    }

    .ck-content p+.image-style-align-left,
    .ck-content p+.image-style-align-right,
    .ck-content p+.image-style-side {
    margin-top: 0;
    }

    .ck-content .image-inline.image-style-align-left,
    .ck-content .image-inline.image-style-align-right {
    margin-bottom: var(--ck-inline-image-style-spacing);
    margin-top: var(--ck-inline-image-style-spacing);
    }

    .ck-content .image-inline.image-style-align-left {
    margin-right: var(--ck-inline-image-style-spacing);
    }

    .ck-content .image-inline.image-style-align-right {
    margin-left: var(--ck-inline-image-style-spacing);
    }

    .ck.ck-splitbutton.ck-splitbutton_flatten.ck-splitbutton_open>.ck-splitbutton__action:not(.ck-disabled),
    .ck.ck-splitbutton.ck-splitbutton_flatten.ck-splitbutton_open>.ck-splitbutton__arrow:not(.ck-disabled),
    .ck.ck-splitbutton.ck-splitbutton_flatten.ck-splitbutton_open>.ck-splitbutton__arrow:not(.ck-disabled):not(:hover),
    .ck.ck-splitbutton.ck-splitbutton_flatten:hover>.ck-splitbutton__action:not(.ck-disabled),
    .ck.ck-splitbutton.ck-splitbutton_flatten:hover>.ck-splitbutton__arrow:not(.ck-disabled),
    .ck.ck-splitbutton.ck-splitbutton_flatten:hover>.ck-splitbutton__arrow:not(.ck-disabled):not(:hover) {
    background-color: var(--ck-color-button-on-background);
    }

    .ck.ck-splitbutton.ck-splitbutton_flatten.ck-splitbutton_open>.ck-splitbutton__action:not(.ck-disabled):after,
    .ck.ck-splitbutton.ck-splitbutton_flatten.ck-splitbutton_open>.ck-splitbutton__arrow:not(.ck-disabled):after,
    .ck.ck-splitbutton.ck-splitbutton_flatten.ck-splitbutton_open>.ck-splitbutton__arrow:not(.ck-disabled):not(:hover):after,
    .ck.ck-splitbutton.ck-splitbutton_flatten:hover>.ck-splitbutton__action:not(.ck-disabled):after,
    .ck.ck-splitbutton.ck-splitbutton_flatten:hover>.ck-splitbutton__arrow:not(.ck-disabled):after,
    .ck.ck-splitbutton.ck-splitbutton_flatten:hover>.ck-splitbutton__arrow:not(.ck-disabled):not(:hover):after {
    display: none;
    }

    .ck.ck-splitbutton.ck-splitbutton_flatten.ck-splitbutton_open:hover>.ck-splitbutton__action:not(.ck-disabled),
    .ck.ck-splitbutton.ck-splitbutton_flatten.ck-splitbutton_open:hover>.ck-splitbutton__arrow:not(.ck-disabled),
    .ck.ck-splitbutton.ck-splitbutton_flatten.ck-splitbutton_open:hover>.ck-splitbutton__arrow:not(.ck-disabled):not(:hover) {
    background-color: var(--ck-color-button-on-hover-background);
    }

    .ck .ck-link_selected {
    background: var(--ck-color-link-selected-background);
    }

    .ck .ck-link_selected span.image-inline {
    outline: var(--ck-widget-outline-thickness) solid var(--ck-color-link-selected-background);
    }

    .ck .ck-fake-link-selection {
    background: var(--ck-color-link-fake-selection);
    }

    .ck .ck-fake-link-selection_collapsed {
    border-right: 1px solid var(--ck-color-base-text);
    height: 100%;
    margin-right: -1px;
    outline: 1px solid hsla(0, 0%, 100%, 0.5);
    }

    .ck.ck-link-form {
    display: flex;
    }

    .ck.ck-link-form .ck-label {
    display: none;
    }

    @media screen and (max-width: 600px) {
    .ck.ck-link-form {
        flex-wrap: wrap;
    }

    .ck.ck-link-form .ck-labeled-field-view {
        flex-basis: 100%;
    }

    .ck.ck-link-form .ck-button {
        flex-basis: 50%;
    }
    }

    .ck.ck-link-form_layout-vertical {
    display: block;
    }

    .ck.ck-link-form_layout-vertical .ck-button.ck-button-cancel,
    .ck.ck-link-form_layout-vertical .ck-button.ck-button-save {
    margin-top: var(--ck-spacing-medium);
    }

    .ck.ck-link-form_layout-vertical {
    min-width: var(--ck-input-width);
    padding: 0;
    }

    .ck.ck-link-form_layout-vertical .ck-labeled-field-view {
    margin: var(--ck-spacing-large) var(--ck-spacing-large) var(--ck-spacing-small);
    }

    .ck.ck-link-form_layout-vertical .ck-labeled-field-view .ck-input-text {
    min-width: 0;
    width: 100%;
    }

    .ck.ck-link-form_layout-vertical>.ck-button {
    border-radius: 0;
    margin: 0;
    padding: var(--ck-spacing-standard);
    width: 50%;
    }

    .ck.ck-link-form_layout-vertical>.ck-button:not(:focus) {
    border-top: 1px solid var(--ck-color-base-border);
    }

    [dir='ltr'] .ck.ck-link-form_layout-vertical>.ck-button,
    [dir='rtl'] .ck.ck-link-form_layout-vertical>.ck-button {
    margin-left: 0;
    }

    [dir='rtl'] .ck.ck-link-form_layout-vertical>.ck-button:last-of-type {
    border-right: 1px solid var(--ck-color-base-border);
    }

    .ck.ck-link-form_layout-vertical .ck.ck-list {
    margin: var(--ck-spacing-standard) var(--ck-spacing-large);
    }

    .ck.ck-link-form_layout-vertical .ck.ck-list .ck-button.ck-switchbutton {
    padding: 0;
    width: 100%;
    }

    .ck.ck-link-form_layout-vertical .ck.ck-list .ck-button.ck-switchbutton:hover {
    background: none;
    }

    .ck.ck-link-actions {
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    }

    .ck.ck-link-actions .ck-link-actions__preview {
    display: inline-block;
    }

    .ck.ck-link-actions .ck-link-actions__preview .ck-button__label {
    overflow: hidden;
    }

    @media screen and (max-width: 600px) {
    .ck.ck-link-actions {
        flex-wrap: wrap;
    }

    .ck.ck-link-actions .ck-link-actions__preview {
        flex-basis: 100%;
    }

    .ck.ck-link-actions .ck-button:not(.ck-link-actions__preview) {
        flex-basis: 50%;
    }
    }

    .ck.ck-link-actions .ck-button.ck-link-actions__preview {
    padding-left: 0;
    padding-right: 0;
    }

    .ck.ck-link-actions .ck-button.ck-link-actions__preview .ck-button__label {
    color: var(--ck-color-link-default);
    cursor: pointer;
    max-width: var(--ck-input-width);
    min-width: 3em;
    padding: 0 var(--ck-spacing-medium);
    text-align: center;
    text-overflow: ellipsis;
    }

    .ck.ck-link-actions .ck-button.ck-link-actions__preview .ck-button__label:hover {
    text-decoration: underline;
    }

    .ck.ck-link-actions .ck-button.ck-link-actions__preview,
    .ck.ck-link-actions .ck-button.ck-link-actions__preview:active,
    .ck.ck-link-actions .ck-button.ck-link-actions__preview:focus,
    .ck.ck-link-actions .ck-button.ck-link-actions__preview:hover {
    background: none;
    }

    .ck.ck-link-actions .ck-button.ck-link-actions__preview:active {
    box-shadow: none;
    }

    .ck.ck-link-actions .ck-button.ck-link-actions__preview:focus .ck-button__label {
    text-decoration: underline;
    }

    [dir='ltr'] .ck.ck-link-actions .ck-button:not(:first-child),
    [dir='rtl'] .ck.ck-link-actions .ck-button:not(:last-child) {
    margin-left: var(--ck-spacing-standard);
    }

    @media screen and (max-width: 600px) {
    .ck.ck-link-actions .ck-button.ck-link-actions__preview {
        margin: var(--ck-spacing-standard) var(--ck-spacing-standard) 0;
    }

    .ck.ck-link-actions .ck-button.ck-link-actions__preview .ck-button__label {
        max-width: 100%;
        min-width: 0;
    }

    [dir='ltr'] .ck.ck-link-actions .ck-button:not(.ck-link-actions__preview),
    [dir='rtl'] .ck.ck-link-actions .ck-button:not(.ck-link-actions__preview) {
        margin-left: 0;
    }
    }

    .ck.ck-editor__editable a span.image-inline:after,
    .ck.ck-editor__editable figure.image>a:after {
    display: block;
    position: absolute;
    }

    :root {
    --ck-link-image-indicator-icon-size: 20;
    --ck-link-image-indicator-icon-is-visible: clamp(0px, 100% - 50px, 1px);
    }

    .ck.ck-editor__editable a span.image-inline:after,
    .ck.ck-editor__editable figure.image>a:after {
    background-color: rgba(0, 0, 0, 0.4);
    background-image: url('data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjAgMjAiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PHBhdGggZmlsbD0iI2ZmZiIgZD0ibTExLjA3NyAxNSAuOTkxLTEuNDE2YS43NS43NSAwIDEgMSAxLjIyOS44NmwtMS4xNDggMS42NGEuNzQ4Ljc0OCAwIDAgMS0uMjE3LjIwNiA1LjI1MSA1LjI1MSAwIDAgMS04LjUwMy01Ljk1NS43NDEuNzQxIDAgMCAxIC4xMi0uMjc0bDEuMTQ3LTEuNjM5YS43NS43NSAwIDEgMSAxLjIyOC44Nkw0LjkzMyAxMC43bC4wMDYuMDAzYTMuNzUgMy43NSAwIDAgMCA2LjEzMiA0LjI5NGwuMDA2LjAwNHptNS40OTQtNS4zMzVhLjc0OC43NDggMCAwIDEtLjEyLjI3NGwtMS4xNDcgMS42MzlhLjc1Ljc1IDAgMSAxLTEuMjI4LS44NmwuODYtMS4yM2EzLjc1IDMuNzUgMCAwIDAtNi4xNDQtNC4zMDFsLS44NiAxLjIyOWEuNzUuNzUgMCAwIDEtMS4yMjktLjg2bDEuMTQ4LTEuNjRhLjc0OC43NDggMCAwIDEgLjIxNy0uMjA2IDUuMjUxIDUuMjUxIDAgMCAxIDguNTAzIDUuOTU1em0tNC41NjMtMi41MzJhLjc1Ljc1IDAgMCAxIC4xODQgMS4wNDVsLTMuMTU1IDQuNTA1YS43NS43NSAwIDEgMS0xLjIyOS0uODZsMy4xNTUtNC41MDZhLjc1Ljc1IDAgMCAxIDEuMDQ1LS4xODR6Ii8+PC9zdmc+');
    background-position: 50%;
    background-repeat: no-repeat;
    background-size: 14px;
    border-radius: 100%;
    content: '';
    height: calc(var(--ck-link-image-indicator-icon-is-visible) * var(--ck-link-image-indicator-icon-size));
    overflow: hidden;
    right: min(var(--ck-spacing-medium), 6%);
    top: min(var(--ck-spacing-medium), 6%);
    width: calc(var(--ck-link-image-indicator-icon-is-visible) * var(--ck-link-image-indicator-icon-size));
    }

    .ck-editor__editable .ck-list-bogus-paragraph {
    display: block;
    }

    .ck-content ol {
    list-style-type: decimal;
    }

    .ck-content ol ol {
    list-style-type: lower-latin;
    }

    .ck-content ol ol ol {
    list-style-type: lower-roman;
    }

    .ck-content ol ol ol ol {
    list-style-type: upper-latin;
    }

    .ck-content ol ol ol ol ol {
    list-style-type: upper-roman;
    }

    .ck-content ul {
    list-style-type: disc;
    }

    .ck-content ul ul {
    list-style-type: circle;
    }

    .ck-content ul ul ul,
    .ck-content ul ul ul ul {
    list-style-type: square;
    }

    .ck.ck-list-properties.ck-list-properties_without-styles {
    padding: var(--ck-spacing-large);
    }

    .ck.ck-list-properties.ck-list-properties_without-styles>* {
    min-width: 14em;
    }

    .ck.ck-list-properties.ck-list-properties_without-styles>*+* {
    margin-top: var(--ck-spacing-standard);
    }

    .ck.ck-list-properties.ck-list-properties_with-numbered-properties>.ck-list-styles-list {
    grid-template-columns: repeat(4, auto);
    }

    .ck.ck-list-properties.ck-list-properties_with-numbered-properties>.ck-collapsible {
    border-top: 1px solid var(--ck-color-base-border);
    }

    .ck.ck-list-properties.ck-list-properties_with-numbered-properties>.ck-collapsible>.ck-collapsible__children>* {
    width: 100%;
    }

    .ck.ck-list-properties.ck-list-properties_with-numbered-properties>.ck-collapsible>.ck-collapsible__children>*+* {
    margin-top: var(--ck-spacing-standard);
    }

    .ck.ck-list-properties .ck.ck-numbered-list-properties__start-index .ck-input {
    min-width: auto;
    width: 100%;
    }

    .ck.ck-list-properties .ck.ck-numbered-list-properties__reversed-order {
    background: transparent;
    margin-bottom: calc(var(--ck-spacing-tiny) * -1);
    padding-left: 0;
    padding-right: 0;
    }

    .ck.ck-list-properties .ck.ck-numbered-list-properties__reversed-order:active,
    .ck.ck-list-properties .ck.ck-numbered-list-properties__reversed-order:hover {
    background: none;
    border-color: transparent;
    box-shadow: none;
    }

    .ck.ck-list-styles-list {
    display: grid;
    }

    :root {
    --ck-list-style-button-size: 44px;
    }

    .ck.ck-list-styles-list {
    column-gap: var(--ck-spacing-medium);
    grid-template-columns: repeat(3, auto);
    padding: var(--ck-spacing-large);
    row-gap: var(--ck-spacing-medium);
    }

    .ck.ck-list-styles-list .ck-button {
    box-sizing: content-box;
    margin: 0;
    padding: 0;
    }

    .ck.ck-list-styles-list .ck-button,
    .ck.ck-list-styles-list .ck-button .ck-icon {
    height: var(--ck-list-style-button-size);
    width: var(--ck-list-style-button-size);
    }

    :root {
    --ck-todo-list-checkmark-size: 16px;
    }

    .ck-content .todo-list {
    list-style: none;
    }

    .ck-content .todo-list li {
    margin-bottom: 5px;
    position: relative;
    }

    .ck-content .todo-list li .todo-list {
    margin-top: 5px;
    }

    .ck-content .todo-list .todo-list__label>input {
    -webkit-appearance: none;
    border: 0;
    display: inline-block;
    height: var(--ck-todo-list-checkmark-size);
    left: -25px;
    margin-left: 0;
    margin-right: -15px;
    position: relative;
    right: 0;
    vertical-align: middle;
    width: var(--ck-todo-list-checkmark-size);
    }

    .ck-content[dir='rtl'] .todo-list .todo-list__label>input {
    left: 0;
    margin-left: -15px;
    margin-right: 0;
    right: -25px;
    }

    .ck-content .todo-list .todo-list__label>input:before {
    border: 1px solid #333;
    border-radius: 2px;
    box-sizing: border-box;
    content: '';
    display: block;
    height: 100%;
    position: absolute;
    transition: box-shadow 0.25s ease-in-out;
    width: 100%;
    }

    .ck-content .todo-list .todo-list__label>input:after {
    border-color: transparent;
    border-style: solid;
    border-width: 0 calc(var(--ck-todo-list-checkmark-size) / 8) calc(var(--ck-todo-list-checkmark-size) / 8) 0;
    box-sizing: content-box;
    content: '';
    display: block;
    height: calc(var(--ck-todo-list-checkmark-size) / 2.6);
    left: calc(var(--ck-todo-list-checkmark-size) / 3);
    pointer-events: none;
    position: absolute;
    top: calc(var(--ck-todo-list-checkmark-size) / 5.3);
    transform: rotate(45deg);
    width: calc(var(--ck-todo-list-checkmark-size) / 5.3);
    }

    .ck-content .todo-list .todo-list__label>input[checked]:before {
    background: #26ab33;
    border-color: #26ab33;
    }

    .ck-content .todo-list .todo-list__label>input[checked]:after {
    border-color: #fff;
    }

    .ck-content .todo-list .todo-list__label .todo-list__label__description {
    vertical-align: middle;
    }

    .ck-content .todo-list .todo-list__label.todo-list__label_without-description input[type='checkbox'] {
    position: absolute;
    }

    .ck-editor__editable.ck-content .todo-list .todo-list__label>input,
    .ck-editor__editable.ck-content .todo-list .todo-list__label>span[contenteditable='false']>input {
    cursor: pointer;
    }

    .ck-editor__editable.ck-content .todo-list .todo-list__label>input:hover:before,
    .ck-editor__editable.ck-content .todo-list .todo-list__label>span[contenteditable='false']>input:hover:before {
    box-shadow: 0 0 0 5px rgba(0, 0, 0, 0.1);
    }

    .ck-editor__editable.ck-content .todo-list .todo-list__label>span[contenteditable='false']>input {
    -webkit-appearance: none;
    border: 0;
    display: inline-block;
    height: var(--ck-todo-list-checkmark-size);
    left: -25px;
    margin-left: 0;
    margin-right: -15px;
    position: relative;
    right: 0;
    vertical-align: middle;
    width: var(--ck-todo-list-checkmark-size);
    }

    .ck-editor__editable.ck-content[dir='rtl'] .todo-list .todo-list__label>span[contenteditable='false']>input {
    left: 0;
    margin-left: -15px;
    margin-right: 0;
    right: -25px;
    }

    .ck-editor__editable.ck-content .todo-list .todo-list__label>span[contenteditable='false']>input:before {
    border: 1px solid #333;
    border-radius: 2px;
    box-sizing: border-box;
    content: '';
    display: block;
    height: 100%;
    position: absolute;
    transition: box-shadow 0.25s ease-in-out;
    width: 100%;
    }

    .ck-editor__editable.ck-content .todo-list .todo-list__label>span[contenteditable='false']>input:after {
    border-color: transparent;
    border-style: solid;
    border-width: 0 calc(var(--ck-todo-list-checkmark-size) / 8) calc(var(--ck-todo-list-checkmark-size) / 8) 0;
    box-sizing: content-box;
    content: '';
    display: block;
    height: calc(var(--ck-todo-list-checkmark-size) / 2.6);
    left: calc(var(--ck-todo-list-checkmark-size) / 3);
    pointer-events: none;
    position: absolute;
    top: calc(var(--ck-todo-list-checkmark-size) / 5.3);
    transform: rotate(45deg);
    width: calc(var(--ck-todo-list-checkmark-size) / 5.3);
    }

    .ck-editor__editable.ck-content .todo-list .todo-list__label>span[contenteditable='false']>input[checked]:before {
    background: #26ab33;
    border-color: #26ab33;
    }

    .ck-editor__editable.ck-content .todo-list .todo-list__label>span[contenteditable='false']>input[checked]:after {
    border-color: #fff;
    }

    .ck-editor__editable.ck-content .todo-list .todo-list__label.todo-list__label_without-description input[type='checkbox'] {
    position: absolute;
    }

    .ck-media__wrapper .ck-media__placeholder {
    align-items: center;
    display: flex;
    flex-direction: column;
    }

    .ck-media__wrapper .ck-media__placeholder .ck-media__placeholder__url {
    max-width: 100%;
    position: relative;
    }

    .ck-media__wrapper .ck-media__placeholder .ck-media__placeholder__url .ck-media__placeholder__url__text {
    display: block;
    overflow: hidden;
    }

    .ck-media__wrapper[data-oembed-url*='facebook.com'] .ck-media__placeholder__icon *,
    .ck-media__wrapper[data-oembed-url*='goo.gl/maps'] .ck-media__placeholder__icon *,
    .ck-media__wrapper[data-oembed-url*='google.com/maps'] .ck-media__placeholder__icon *,
    .ck-media__wrapper[data-oembed-url*='instagram.com'] .ck-media__placeholder__icon *,
    .ck-media__wrapper[data-oembed-url*='maps.app.goo.gl'] .ck-media__placeholder__icon *,
    .ck-media__wrapper[data-oembed-url*='maps.google.com'] .ck-media__placeholder__icon *,
    .ck-media__wrapper[data-oembed-url*='twitter.com'] .ck-media__placeholder__icon * {
    display: none;
    }

    .ck-editor__editable:not(.ck-read-only) .ck-media__wrapper> :not(.ck-media__placeholder),
    .ck-editor__editable:not(.ck-read-only) .ck-widget:not(.ck-widget_selected) .ck-media__placeholder {
    pointer-events: none;
    }

    :root {
    --ck-media-embed-placeholder-icon-size: 3em;
    --ck-color-media-embed-placeholder-url-text: #757575;
    --ck-color-media-embed-placeholder-url-text-hover: var(--ck-color-base-text);
    }

    .ck-media__wrapper {
    margin: 0 auto;
    }

    .ck-media__wrapper .ck-media__placeholder {
    background: var(--ck-color-base-foreground);
    padding: calc(var(--ck-spacing-standard) * 3);
    }

    .ck-media__wrapper .ck-media__placeholder .ck-media__placeholder__icon {
    background-position: 50%;
    background-size: cover;
    height: var(--ck-media-embed-placeholder-icon-size);
    margin-bottom: var(--ck-spacing-large);
    min-width: var(--ck-media-embed-placeholder-icon-size);
    }

    .ck-media__wrapper .ck-media__placeholder .ck-media__placeholder__icon .ck-icon {
    height: 100%;
    width: 100%;
    }

    .ck-media__wrapper .ck-media__placeholder .ck-media__placeholder__url__text {
    color: var(--ck-color-media-embed-placeholder-url-text);
    font-style: italic;
    text-align: center;
    text-overflow: ellipsis;
    white-space: nowrap;
    }

    .ck-media__wrapper .ck-media__placeholder .ck-media__placeholder__url__text:hover {
    color: var(--ck-color-media-embed-placeholder-url-text-hover);
    cursor: pointer;
    text-decoration: underline;
    }

    .ck-media__wrapper[data-oembed-url*='open.spotify.com'] {
    max-height: 380px;
    max-width: 300px;
    }

    .ck-media__wrapper[data-oembed-url*='goo.gl/maps'] .ck-media__placeholder__icon,
    .ck-media__wrapper[data-oembed-url*='google.com/maps'] .ck-media__placeholder__icon,
    .ck-media__wrapper[data-oembed-url*='maps.app.goo.gl'] .ck-media__placeholder__icon,
    .ck-media__wrapper[data-oembed-url*='maps.google.com'] .ck-media__placeholder__icon {
    background-image: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNTAuMzc4IiBoZWlnaHQ9IjI1NC4xNjciIHZpZXdCb3g9IjAgMCA2Ni4yNDYgNjcuMjQ4Ij48ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTcyLjUzMSAtMjE4LjQ1NSkgc2NhbGUoLjk4MDEyKSI+PHJlY3Qgcnk9IjUuMjM4IiByeD0iNS4yMzgiIHk9IjIzMS4zOTkiIHg9IjE3Ni4wMzEiIGhlaWdodD0iNjAuMDk5IiB3aWR0aD0iNjAuMDk5IiBmaWxsPSIjMzRhNjY4IiBwYWludC1vcmRlcj0ibWFya2VycyBzdHJva2UgZmlsbCIvPjxwYXRoIGQ9Im0yMDYuNDc3IDI2MC45LTI4Ljk4NyAyOC45ODdhNS4yMTggNS4yMTggMCAwIDAgMy43OCAxLjYxaDQ5LjYyMWMxLjY5NCAwIDMuMTktLjc5OCA0LjE0Ni0yLjAzN3oiIGZpbGw9IiM1Yzg4YzUiLz48cGF0aCBkPSJNMjI2Ljc0MiAyMjIuOTg4Yy05LjI2NiAwLTE2Ljc3NyA3LjE3LTE2Ljc3NyAxNi4wMTQuMDA3IDIuNzYyLjY2MyA1LjQ3NCAyLjA5MyA3Ljg3NS40My43MDMuODMgMS40MDggMS4xOSAyLjEwNy4zMzMuNTAyLjY1IDEuMDA1Ljk1IDEuNTA4LjM0My40NzcuNjczLjk1Ny45ODggMS40NCAxLjMxIDEuNzY5IDIuNSAzLjUwMiAzLjYzNyA1LjE2OC43OTMgMS4yNzUgMS42ODMgMi42NCAyLjQ2NiAzLjk5IDIuMzYzIDQuMDk0IDQuMDA3IDguMDkyIDQuNiAxMy45MTR2LjAxMmMuMTgyLjQxMi41MTYuNjY2Ljg3OS42NjcuNDAzLS4wMDEuNzY4LS4zMTQuOTMtLjc5OS42MDMtNS43NTYgMi4yMzgtOS43MjkgNC41ODUtMTMuNzk0Ljc4Mi0xLjM1IDEuNjczLTIuNzE1IDIuNDY1LTMuOTkgMS4xMzctMS42NjYgMi4zMjgtMy40IDMuNjM4LTUuMTY5LjMxNS0uNDgyLjY0NS0uOTYyLjk4OC0xLjQzOS4zLS41MDMuNjE3LTEuMDA2Ljk1LTEuNTA4LjM1OS0uNy43Ni0xLjQwNCAxLjE5LTIuMTA3IDEuNDI2LTIuNDAyIDItNS4xMTQgMi4wMDQtNy44NzUgMC04Ljg0NC03LjUxMS0xNi4wMTQtMTYuNzc2LTE2LjAxNHoiIGZpbGw9IiNkZDRiM2UiIHBhaW50LW9yZGVyPSJtYXJrZXJzIHN0cm9rZSBmaWxsIi8+PGVsbGlwc2Ugcnk9IjUuNTY0IiByeD0iNS44MjgiIGN5PSIyMzkuMDAyIiBjeD0iMjI2Ljc0MiIgZmlsbD0iIzgwMmQyNyIgcGFpbnQtb3JkZXI9Im1hcmtlcnMgc3Ryb2tlIGZpbGwiLz48cGF0aCBkPSJNMTkwLjMwMSAyMzcuMjgzYy00LjY3IDAtOC40NTcgMy44NTMtOC40NTcgOC42MDZzMy43ODYgOC42MDcgOC40NTcgOC42MDdjMy4wNDMgMCA0LjgwNi0uOTU4IDYuMzM3LTIuNTE2IDEuNTMtMS41NTcgMi4wODctMy45MTMgMi4wODctNi4yOSAwLS4zNjItLjAyMy0uNzIyLS4wNjQtMS4wNzloLTguMjU3djMuMDQzaDQuODVjLS4xOTcuNzU5LS41MzEgMS40NS0xLjA1OCAxLjk4Ni0uOTQyLjk1OC0yLjAyOCAxLjU0OC0zLjkwMSAxLjU0OC0yLjg3NiAwLTUuMjA4LTIuMzcyLTUuMjA4LTUuMjk5IDAtMi45MjYgMi4zMzItNS4yOTkgNS4yMDgtNS4yOTkgMS4zOTkgMCAyLjYxOC40MDcgMy41ODQgMS4yOTNsMi4zODEtMi4zOGMwLS4wMDItLjAwMy0uMDA0LS4wMDQtLjAwNS0xLjU4OC0xLjUyNC0zLjYyLTIuMjE1LTUuOTU1LTIuMjE1em00LjQzIDUuNjYuMDAzLjAwNnYtLjAwM3oiIGZpbGw9IiNmZmYiIHBhaW50LW9yZGVyPSJtYXJrZXJzIHN0cm9rZSBmaWxsIi8+PHBhdGggZD0ibTIxNS4xODQgMjUxLjkyOS03Ljk4IDcuOTc5IDI4LjQ3NyAyOC40NzVhNS4yMzMgNS4yMzMgMCAwIDAgLjQ0OS0yLjEyM3YtMzEuMTY1Yy0uNDY5LjY3NS0uOTM0IDEuMzQ5LTEuMzgyIDIuMDA1LS43OTIgMS4yNzUtMS42ODIgMi42NC0yLjQ2NSAzLjk5LTIuMzQ3IDQuMDY1LTMuOTgyIDguMDM4LTQuNTg1IDEzLjc5NC0uMTYyLjQ4NS0uNTI3Ljc5OC0uOTMuNzk5LS4zNjMtLjAwMS0uNjk3LS4yNTUtLjg3OS0uNjY3di0uMDEyYy0uNTkzLTUuODIyLTIuMjM3LTkuODItNC42LTEzLjkxNC0uNzgzLTEuMzUtMS42NzMtMi43MTUtMi40NjYtMy45OS0xLjEzNy0xLjY2Ni0yLjMyNy0zLjQtMy42MzctNS4xNjlsLS4wMDItLjAwM3oiIGZpbGw9IiNjM2MzYzMiLz48cGF0aCBkPSJtMjEyLjk4MyAyNDguNDk1LTM2Ljk1MiAzNi45NTN2LjgxMmE1LjIyNyA1LjIyNyAwIDAgMCA1LjIzOCA1LjIzOGgxLjAxNWwzNS42NjYtMzUuNjY2YTEzNi4yNzUgMTM2LjI3NSAwIDAgMC0yLjc2NC0zLjkgMzcuNTc1IDM3LjU3NSAwIDAgMC0uOTg5LTEuNDQgMzUuMTI3IDM1LjEyNyAwIDAgMC0uOTUtMS41MDhjLS4wODMtLjE2Mi0uMTc2LS4zMjYtLjI2NC0uNDg5eiIgZmlsbD0iI2ZkZGM0ZiIgcGFpbnQtb3JkZXI9Im1hcmtlcnMgc3Ryb2tlIGZpbGwiLz48cGF0aCBkPSJtMjExLjk5OCAyNjEuMDgzLTYuMTUyIDYuMTUxIDI0LjI2NCAyNC4yNjRoLjc4MWE1LjIyNyA1LjIyNyAwIDAgMCA1LjIzOS01LjIzOHYtMS4wNDV6IiBmaWxsPSIjZmZmIiBwYWludC1vcmRlcj0ibWFya2VycyBzdHJva2UgZmlsbCIvPjwvZz48L3N2Zz4=);
    }

    .ck-media__wrapper[data-oembed-url*='facebook.com'] .ck-media__placeholder {
    background: #4268b3;
    }

    .ck-media__wrapper[data-oembed-url*='facebook.com'] .ck-media__placeholder .ck-media__placeholder__icon {
    background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTAyNCIgaGVpZ2h0PSIxMDI0IiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPjxwYXRoIGQ9Ik05NjcuNDg0IDBINTYuNTE3QzI1LjMwNCAwIDAgMjUuMzA0IDAgNTYuNTE3djkxMC45NjZDMCA5OTguNjk0IDI1LjI5NyAxMDI0IDU2LjUyMiAxMDI0SDU0N1Y2MjhINDE0VjQ3M2gxMzNWMzU5LjAyOWMwLTEzMi4yNjIgODAuNzczLTIwNC4yODIgMTk4Ljc1Ni0yMDQuMjgyIDU2LjUxMyAwIDEwNS4wODYgNC4yMDggMTE5LjI0NCA2LjA4OVYyOTlsLTgxLjYxNi4wMzdjLTYzLjk5MyAwLTc2LjM4NCAzMC40OTItNzYuMzg0IDc1LjIzNlY0NzNoMTUzLjQ4N2wtMTkuOTg2IDE1NUg3MDd2Mzk2aDI2MC40ODRjMzEuMjEzIDAgNTYuNTE2LTI1LjMwMyA1Ni41MTYtNTYuNTE2VjU2LjUxNUMxMDI0IDI1LjMwMyA5OTguNjk3IDAgOTY3LjQ4NCAwIiBmaWxsPSIjRkZGRkZFIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiLz48L3N2Zz4=);
    }

    .ck-media__wrapper[data-oembed-url*='facebook.com'] .ck-media__placeholder .ck-media__placeholder__url__text {
    color: #cdf;
    }

    .ck-media__wrapper[data-oembed-url*='facebook.com'] .ck-media__placeholder .ck-media__placeholder__url__text:hover {
    color: #fff;
    }

    .ck-media__wrapper[data-oembed-url*='instagram.com'] .ck-media__placeholder {
    background: linear-gradient(-135deg, #1400c7, #b800b1, #f50000);
    }

    .ck-media__wrapper[data-oembed-url*='instagram.com'] .ck-media__placeholder .ck-media__placeholder__icon {
    background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNTA0IiBoZWlnaHQ9IjUwNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayI+PGRlZnM+PHBhdGggaWQ9ImEiIGQ9Ik0wIC4xNTloNTAzLjg0MVY1MDMuOTRIMHoiLz48L2RlZnM+PGcgZmlsbD0ibm9uZSIgZmlsbC1ydWxlPSJldmVub2RkIj48bWFzayBpZD0iYiIgZmlsbD0iI2ZmZiI+PHVzZSB4bGluazpocmVmPSIjYSIvPjwvbWFzaz48cGF0aCBkPSJNMjUxLjkyMS4xNTljLTY4LjQxOCAwLTc2Ljk5Ny4yOS0xMDMuODY3IDEuNTE2LTI2LjgxNCAxLjIyMy00NS4xMjcgNS40ODItNjEuMTUxIDExLjcxLTE2LjU2NiA2LjQzNy0zMC42MTUgMTUuMDUxLTQ0LjYyMSAyOS4wNTYtMTQuMDA1IDE0LjAwNi0yMi42MTkgMjguMDU1LTI5LjA1NiA0NC42MjEtNi4yMjggMTYuMDI0LTEwLjQ4NyAzNC4zMzctMTEuNzEgNjEuMTUxQy4yOSAxNzUuMDgzIDAgMTgzLjY2MiAwIDI1Mi4wOGMwIDY4LjQxNy4yOSA3Ni45OTYgMS41MTYgMTAzLjg2NiAxLjIyMyAyNi44MTQgNS40ODIgNDUuMTI3IDExLjcxIDYxLjE1MSA2LjQzNyAxNi41NjYgMTUuMDUxIDMwLjYxNSAyOS4wNTYgNDQuNjIxIDE0LjAwNiAxNC4wMDUgMjguMDU1IDIyLjYxOSA0NC42MjEgMjkuMDU3IDE2LjAyNCA2LjIyNyAzNC4zMzcgMTAuNDg2IDYxLjE1MSAxMS43MDkgMjYuODcgMS4yMjYgMzUuNDQ5IDEuNTE2IDEwMy44NjcgMS41MTYgNjguNDE3IDAgNzYuOTk2LS4yOSAxMDMuODY2LTEuNTE2IDI2LjgxNC0xLjIyMyA0NS4xMjctNS40ODIgNjEuMTUxLTExLjcwOSAxNi41NjYtNi40MzggMzAuNjE1LTE1LjA1MiA0NC42MjEtMjkuMDU3IDE0LjAwNS0xNC4wMDYgMjIuNjE5LTI4LjA1NSAyOS4wNTctNDQuNjIxIDYuMjI3LTE2LjAyNCAxMC40ODYtMzQuMzM3IDExLjcwOS02MS4xNTEgMS4yMjYtMjYuODcgMS41MTYtMzUuNDQ5IDEuNTE2LTEwMy44NjYgMC02OC40MTgtLjI5LTc2Ljk5Ny0xLjUxNi0xMDMuODY3LTEuMjIzLTI2LjgxNC01LjQ4Mi00NS4xMjctMTEuNzA5LTYxLjE1MS02LjQzOC0xNi41NjYtMTUuMDUyLTMwLjYxNS0yOS4wNTctNDQuNjIxLTE0LjAwNi0xNC4wMDUtMjguMDU1LTIyLjYxOS00NC42MjEtMjkuMDU2LTE2LjAyNC02LjIyOC0zNC4zMzctMTAuNDg3LTYxLjE1MS0xMS43MUMzMjguOTE3LjQ0OSAzMjAuMzM4LjE1OSAyNTEuOTIxLjE1OVptMCA0NS4zOTFjNjcuMjY1IDAgNzUuMjMzLjI1NyAxMDEuNzk3IDEuNDY5IDI0LjU2MiAxLjEyIDM3LjkwMSA1LjIyNCA0Ni43NzggOC42NzQgMTEuNzU5IDQuNTcgMjAuMTUxIDEwLjAyOSAyOC45NjYgMTguODQ1IDguODE2IDguODE1IDE0LjI3NSAxNy4yMDcgMTguODQ1IDI4Ljk2NiAzLjQ1IDguODc3IDcuNTU0IDIyLjIxNiA4LjY3NCA0Ni43NzggMS4yMTIgMjYuNTY0IDEuNDY5IDM0LjUzMiAxLjQ2OSAxMDEuNzk4IDAgNjcuMjY1LS4yNTcgNzUuMjMzLTEuNDY5IDEwMS43OTctMS4xMiAyNC41NjItNS4yMjQgMzcuOTAxLTguNjc0IDQ2Ljc3OC00LjU3IDExLjc1OS0xMC4wMjkgMjAuMTUxLTE4Ljg0NSAyOC45NjYtOC44MTUgOC44MTYtMTcuMjA3IDE0LjI3NS0yOC45NjYgMTguODQ1LTguODc3IDMuNDUtMjIuMjE2IDcuNTU0LTQ2Ljc3OCA4LjY3NC0yNi41NiAxLjIxMi0zNC41MjcgMS40NjktMTAxLjc5NyAxLjQ2OS02Ny4yNzEgMC03NS4yMzctLjI1Ny0xMDEuNzk4LTEuNDY5LTI0LjU2Mi0xLjEyLTM3LjkwMS01LjIyNC00Ni43NzgtOC42NzQtMTEuNzU5LTQuNTctMjAuMTUxLTEwLjAyOS0yOC45NjYtMTguODQ1LTguODE1LTguODE1LTE0LjI3NS0xNy4yMDctMTguODQ1LTI4Ljk2Ni0zLjQ1LTguODc3LTcuNTU0LTIyLjIxNi04LjY3NC00Ni43NzgtMS4yMTItMjYuNTY0LTEuNDY5LTM0LjUzMi0xLjQ2OS0xMDEuNzk3IDAtNjcuMjY2LjI1Ny03NS4yMzQgMS40NjktMTAxLjc5OCAxLjEyLTI0LjU2MiA1LjIyNC0zNy45MDEgOC42NzQtNDYuNzc4IDQuNTctMTEuNzU5IDEwLjAyOS0yMC4xNTEgMTguODQ1LTI4Ljk2NiA4LjgxNS04LjgxNiAxNy4yMDctMTQuMjc1IDI4Ljk2Ni0xOC44NDUgOC44NzctMy40NSAyMi4yMTYtNy41NTQgNDYuNzc4LTguNjc0IDI2LjU2NC0xLjIxMiAzNC41MzItMS40NjkgMTAxLjc5OC0xLjQ2OVoiIGZpbGw9IiNGRkYiIG1hc2s9InVybCgjYikiLz48cGF0aCBkPSJNMjUxLjkyMSAzMzYuMDUzYy00Ni4zNzggMC04My45NzQtMzcuNTk2LTgzLjk3NC04My45NzMgMC00Ni4zNzggMzcuNTk2LTgzLjk3NCA4My45NzQtODMuOTc0IDQ2LjM3NyAwIDgzLjk3MyAzNy41OTYgODMuOTczIDgzLjk3NCAwIDQ2LjM3Ny0zNy41OTYgODMuOTczLTgzLjk3MyA4My45NzNabTAtMjEzLjMzOGMtNzEuNDQ3IDAtMTI5LjM2NSA1Ny45MTgtMTI5LjM2NSAxMjkuMzY1IDAgNzEuNDQ2IDU3LjkxOCAxMjkuMzY0IDEyOS4zNjUgMTI5LjM2NCA3MS40NDYgMCAxMjkuMzY0LTU3LjkxOCAxMjkuMzY0LTEyOS4zNjQgMC03MS40NDctNTcuOTE4LTEyOS4zNjUtMTI5LjM2NC0xMjkuMzY1Wk00MTYuNjI3IDExNy42MDRjMCAxNi42OTYtMTMuNTM1IDMwLjIzLTMwLjIzMSAzMC4yMy0xNi42OTUgMC0zMC4yMy0xMy41MzQtMzAuMjMtMzAuMjMgMC0xNi42OTYgMTMuNTM1LTMwLjIzMSAzMC4yMy0zMC4yMzEgMTYuNjk2IDAgMzAuMjMxIDEzLjUzNSAzMC4yMzEgMzAuMjMxIiBmaWxsPSIjRkZGIi8+PC9nPjwvc3ZnPg==);
    }

    .ck-media__wrapper[data-oembed-url*='instagram.com'] .ck-media__placeholder .ck-media__placeholder__url__text {
    color: #ffe0fe;
    }

    .ck-media__wrapper[data-oembed-url*='instagram.com'] .ck-media__placeholder .ck-media__placeholder__url__text:hover {
    color: #fff;
    }

    .ck-media__wrapper[data-oembed-url*='twitter.com'] .ck.ck-media__placeholder {
    background: linear-gradient(90deg, #71c6f4, #0d70a5);
    }

    .ck-media__wrapper[data-oembed-url*='twitter.com'] .ck.ck-media__placeholder .ck-media__placeholder__icon {
    background-image: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA0MDAgNDAwIiBzdHlsZT0iZW5hYmxlLWJhY2tncm91bmQ6bmV3IDAgMCA0MDAgNDAwIiB4bWw6c3BhY2U9InByZXNlcnZlIj48cGF0aCBkPSJNNDAwIDIwMGMwIDExMC41LTg5LjUgMjAwLTIwMCAyMDBTMCAzMTAuNSAwIDIwMCA4OS41IDAgMjAwIDBzMjAwIDg5LjUgMjAwIDIwMHpNMTYzLjQgMzA1LjVjODguNyAwIDEzNy4yLTczLjUgMTM3LjItMTM3LjIgMC0yLjEgMC00LjItLjEtNi4yIDkuNC02LjggMTcuNi0xNS4zIDI0LjEtMjUtOC42IDMuOC0xNy45IDYuNC0yNy43IDcuNiAxMC02IDE3LjYtMTUuNCAyMS4yLTI2LjctOS4zIDUuNS0xOS42IDkuNS0zMC42IDExLjctOC44LTkuNC0yMS4zLTE1LjItMzUuMi0xNS4yLTI2LjYgMC00OC4yIDIxLjYtNDguMiA0OC4yIDAgMy44LjQgNy41IDEuMyAxMS00MC4xLTItNzUuNi0yMS4yLTk5LjQtNTAuNC00LjEgNy4xLTYuNSAxNS40LTYuNSAyNC4yIDAgMTYuNyA4LjUgMzEuNSAyMS41IDQwLjEtNy45LS4yLTE1LjMtMi40LTIxLjgtNnYuNmMwIDIzLjQgMTYuNiA0Mi44IDM4LjcgNDcuMy00IDEuMS04LjMgMS43LTEyLjcgMS43LTMuMSAwLTYuMS0uMy05LjEtLjkgNi4xIDE5LjIgMjMuOSAzMy4xIDQ1IDMzLjUtMTYuNSAxMi45LTM3LjMgMjAuNi01OS45IDIwLjYtMy45IDAtNy43LS4yLTExLjUtLjcgMjEuMSAxMy44IDQ2LjUgMjEuOCA3My43IDIxLjgiIHN0eWxlPSJmaWxsOiNmZmYiLz48L3N2Zz4=);
    }

    .ck-media__wrapper[data-oembed-url*='twitter.com'] .ck.ck-media__placeholder .ck-media__placeholder__url__text {
    color: #b8e6ff;
    }

    .ck-media__wrapper[data-oembed-url*='twitter.com'] .ck.ck-media__placeholder .ck-media__placeholder__url__text:hover {
    color: #fff;
    }

    .ck.ck-media-form {
    align-items: flex-start;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    }

    .ck.ck-media-form .ck-labeled-field-view {
    display: inline-block;
    }

    .ck.ck-media-form .ck-label {
    display: none;
    }

    @media screen and (max-width: 600px) {
    .ck.ck-media-form {
        flex-wrap: wrap;
    }

    .ck.ck-media-form .ck-labeled-field-view {
        flex-basis: 100%;
    }

    .ck.ck-media-form .ck-button {
        flex-basis: 50%;
    }
    }

    .ck-content .media {
    clear: both;
    display: block;
    margin: 0.9em 0;
    min-width: 15em;
    }

    :root {
    --ck-mention-list-max-height: 300px;
    }

    .ck.ck-mentions {
    max-height: var(--ck-mention-list-max-height);
    overflow-x: hidden;
    overflow-y: auto;
    overscroll-behavior: contain;
    }

    .ck.ck-mentions>.ck-list__item {
    flex-shrink: 0;
    overflow: hidden;
    }

    :root {
    --ck-color-mention-background: rgba(153, 0, 48, 0.1);
    --ck-color-mention-text: #990030;
    }

    .ck-content .mention {
    background: var(--ck-color-mention-background);
    color: var(--ck-color-mention-text);
    }

    .ck-content .page-break {
    align-items: center;
    clear: both;
    display: flex;
    justify-content: center;
    padding: 5px 0;
    position: relative;
    }

    .ck-content .page-break:after {
    border-bottom: 2px dashed #c4c4c4;
    content: '';
    position: absolute;
    width: 100%;
    }

    .ck-content .page-break__label {
    background: #fff;
    border: 1px solid #c4c4c4;
    border-radius: 2px;
    box-shadow: 2px 2px 1px rgba(0, 0, 0, 0.15);
    color: #333;
    display: block;
    font-family: Helvetica, Arial, Tahoma, Verdana, Sans-Serif;
    font-size: 0.75em;
    font-weight: 700;
    padding: 0.3em 0.6em;
    position: relative;
    text-transform: uppercase;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
    z-index: 1;
    }

    @media print {
    .ck-content .page-break {
        padding: 0;
    }

    .ck-content .page-break:after {
        display: none;
    }
    }

    :root {
    --ck-color-restricted-editing-exception-background: rgba(255, 169, 77, 0.2);
    --ck-color-restricted-editing-exception-hover-background: rgba(255,
        169,
        77,
        0.35);
    --ck-color-restricted-editing-exception-brackets: rgba(204, 105, 0, 0.4);
    --ck-color-restricted-editing-selected-exception-background: rgba(255,
        169,
        77,
        0.5);
    --ck-color-restricted-editing-selected-exception-brackets: rgba(204,
        105,
        0,
        0.6);
    }

    .ck-editor__editable .restricted-editing-exception {
    background-color: var(--ck-color-restricted-editing-exception-background);
    border: 1px solid;
    border-image: linear-gradient(to right,
        var(--ck-color-restricted-editing-exception-brackets) 0,
        var(--ck-color-restricted-editing-exception-brackets) 5px,
        transparent 6px,
        transparent calc(100% - 6px),
        var(--ck-color-restricted-editing-exception-brackets) calc(100% - 5px),
        var(--ck-color-restricted-editing-exception-brackets) 100%) 1;
    transition: background 0.2s ease-in-out;
    }

    .ck-editor__editable .restricted-editing-exception.restricted-editing-exception_selected {
    background-color: var(--ck-color-restricted-editing-selected-exception-background);
    border-image: linear-gradient(to right,
        var(--ck-color-restricted-editing-selected-exception-brackets) 0,
        var(--ck-color-restricted-editing-selected-exception-brackets) 5px,
        var(--ck-color-restricted-editing-selected-exception-brackets) calc(100% - 5px),
        var(--ck-color-restricted-editing-selected-exception-brackets) 100%) 1;
    }

    .ck-editor__editable .restricted-editing-exception.restricted-editing-exception_collapsed {
    padding-left: 1ch;
    }

    .ck-restricted-editing_mode_restricted,
    .ck-restricted-editing_mode_restricted * {
    cursor: default;
    }

    .ck-restricted-editing_mode_restricted .restricted-editing-exception,
    .ck-restricted-editing_mode_restricted .restricted-editing-exception * {
    cursor: text;
    }

    .ck-restricted-editing_mode_restricted .restricted-editing-exception:hover {
    background: var(--ck-color-restricted-editing-exception-hover-background);
    }

    .ck.ck-character-grid {
    max-width: 100%;
    }

    .ck.ck-character-grid .ck-character-grid__tiles {
    display: grid;
    }

    :root {
    --ck-character-grid-tile-size: 24px;
    }

    .ck.ck-character-grid {
    max-height: 200px;
    overflow-x: hidden;
    overflow-y: auto;
    width: 350px;
    }

    @media screen and (max-width: 600px) {
    .ck.ck-character-grid {
        width: 190px;
    }
    }

    .ck.ck-character-grid .ck-character-grid__tiles {
    grid-gap: var(--ck-spacing-standard);
    grid-template-columns: repeat(10, 1fr);
    margin: var(--ck-spacing-standard) var(--ck-spacing-large);
    }

    @media screen and (max-width: 600px) {
    .ck.ck-character-grid .ck-character-grid__tiles {
        grid-template-columns: repeat(5, 1fr);
    }
    }

    .ck.ck-character-grid .ck-character-grid__tile {
    border: 0;
    font-size: 1.2em;
    height: var(--ck-character-grid-tile-size);
    min-height: var(--ck-character-grid-tile-size);
    min-width: var(--ck-character-grid-tile-size);
    padding: 0;
    transition: box-shadow 0.2s ease;
    width: var(--ck-character-grid-tile-size);
    }

    .ck.ck-character-grid .ck-character-grid__tile:focus:not(.ck-disabled),
    .ck.ck-character-grid .ck-character-grid__tile:hover:not(.ck-disabled) {
    border: 0;
    box-shadow: inset 0 0 0 1px var(--ck-color-base-background),
        0 0 0 2px var(--ck-color-focus-border);
    }

    .ck.ck-character-grid .ck-character-grid__tile .ck-button__label {
    line-height: var(--ck-character-grid-tile-size);
    text-align: center;
    width: 100%;
    }

    .ck.ck-character-info {
    border-top: 1px solid var(--ck-color-base-border);
    display: flex;
    justify-content: space-between;
    padding: var(--ck-spacing-small) var(--ck-spacing-large);
    }

    .ck.ck-character-info>* {
    font-size: var(--ck-font-size-small);
    text-transform: uppercase;
    }

    .ck.ck-character-info .ck-character-info__name {
    max-width: 280px;
    overflow: hidden;
    text-overflow: ellipsis;
    }

    .ck.ck-character-info .ck-character-info__code {
    opacity: 0.6;
    }

    @media screen and (max-width: 600px) {
    .ck.ck-character-info {
        max-width: 190px;
    }
    }

    .ck.ck-special-characters-navigation>.ck-label {
    max-width: 160px;
    overflow: hidden;
    text-overflow: ellipsis;
    }

    .ck.ck-special-characters-navigation>.ck-dropdown .ck-dropdown__panel {
    max-height: 250px;
    overflow-x: hidden;
    overflow-y: auto;
    }

    @media screen and (max-width: 600px) {
    .ck.ck-special-characters-navigation {
        max-width: 190px;
    }

    .ck.ck-special-characters-navigation>.ck-form__header__label {
        overflow: hidden;
        text-overflow: ellipsis;
    }
    }

    :root {
    --ck-color-selector-focused-cell-background: rgba(158, 201, 250, 0.3);
    }

    .ck-widget.table td.ck-editor__nested-editable.ck-editor__nested-editable_focused,
    .ck-widget.table td.ck-editor__nested-editable:focus,
    .ck-widget.table th.ck-editor__nested-editable.ck-editor__nested-editable_focused,
    .ck-widget.table th.ck-editor__nested-editable:focus {
    background: var(--ck-color-selector-focused-cell-background);
    border-style: none;
    outline: 1px solid var(--ck-color-focus-border);
    outline-offset: -1px;
    }

    .ck .ck-insert-table-dropdown__grid {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    }

    :root {
    --ck-insert-table-dropdown-padding: 10px;
    --ck-insert-table-dropdown-box-height: 11px;
    --ck-insert-table-dropdown-box-width: 12px;
    --ck-insert-table-dropdown-box-margin: 1px;
    }

    .ck .ck-insert-table-dropdown__grid {
    padding: var(--ck-insert-table-dropdown-padding) var(--ck-insert-table-dropdown-padding) 0;
    width: calc(var(--ck-insert-table-dropdown-box-width) * 10 + var(--ck-insert-table-dropdown-box-margin) * 20 + var(--ck-insert-table-dropdown-padding) * 2);
    }

    .ck .ck-insert-table-dropdown__label,
    .ck[dir='rtl'] .ck-insert-table-dropdown__label {
    text-align: center;
    }

    .ck .ck-insert-table-dropdown-grid-box {
    border: 1px solid var(--ck-color-base-border);
    border-radius: 1px;
    margin: var(--ck-insert-table-dropdown-box-margin);
    min-height: var(--ck-insert-table-dropdown-box-height);
    min-width: var(--ck-insert-table-dropdown-box-width);
    outline: none;
    transition: none;
    }

    .ck .ck-insert-table-dropdown-grid-box:focus {
    box-shadow: none;
    }

    .ck .ck-insert-table-dropdown-grid-box.ck-on {
    background: var(--ck-color-focus-outer-shadow);
    border-color: var(--ck-color-focus-border);
    }

    :root {
    --ck-table-selected-cell-background: rgba(158, 207, 250, 0.3);
    }

    .ck.ck-editor__editable .table table td.ck-editor__editable_selected,
    .ck.ck-editor__editable .table table th.ck-editor__editable_selected {
    box-shadow: unset;
    caret-color: transparent;
    outline: unset;
    position: relative;
    }

    .ck.ck-editor__editable .table table td.ck-editor__editable_selected:after,
    .ck.ck-editor__editable .table table th.ck-editor__editable_selected:after {
    background-color: var(--ck-table-selected-cell-background);
    bottom: 0;
    content: '';
    left: 0;
    pointer-events: none;
    position: absolute;
    right: 0;
    top: 0;
    }

    .ck.ck-editor__editable .table table td.ck-editor__editable_selected ::selection,
    .ck.ck-editor__editable .table table td.ck-editor__editable_selected:focus,
    .ck.ck-editor__editable .table table th.ck-editor__editable_selected ::selection,
    .ck.ck-editor__editable .table table th.ck-editor__editable_selected:focus {
    background-color: transparent;
    }

    .ck.ck-editor__editable .table table td.ck-editor__editable_selected .ck-widget,
    .ck.ck-editor__editable .table table th.ck-editor__editable_selected .ck-widget {
    outline: unset;
    }

    .ck.ck-editor__editable .table table td.ck-editor__editable_selected .ck-widget>.ck-widget__selection-handle,
    .ck.ck-editor__editable .table table th.ck-editor__editable_selected .ck-widget>.ck-widget__selection-handle {
    display: none;
    }

    .ck-content .table {
    display: table;
    margin: 0.9em auto;
    }

    .ck-content .table table {
    border: 1px double #b3b3b3;
    border-collapse: collapse;
    border-spacing: 0;
    height: 100%;
    width: 100%;
    }

    .ck-content .table table td,
    .ck-content .table table th {
    border: 1px solid #bfbfbf;
    min-width: 2em;
    padding: 0.4em;
    }

    .ck-content .table table th {
    background: rgba(0, 0, 0, 0.05);
    font-weight: 700;
    }

    .ck-content[dir='rtl'] .table th {
    text-align: right;
    }

    .ck-content[dir='ltr'] .table th {
    text-align: left;
    }

    .ck-editor__editable .ck-table-bogus-paragraph {
    display: inline-block;
    width: 100%;
    }

    .ck.ck-input-color {
    display: flex;
    flex-direction: row-reverse;
    width: 100%;
    }

    .ck.ck-input-color>input.ck.ck-input-text {
    flex-grow: 1;
    min-width: auto;
    }

    .ck.ck-input-color>div.ck.ck-dropdown {
    min-width: auto;
    }

    .ck.ck-input-color>div.ck.ck-dropdown>.ck-input-color__button .ck-dropdown__arrow {
    display: none;
    }

    .ck.ck-input-color .ck.ck-input-color__button {
    display: flex;
    }

    .ck.ck-input-color .ck.ck-input-color__button .ck.ck-input-color__button__preview {
    overflow: hidden;
    position: relative;
    }

    .ck.ck-input-color .ck.ck-input-color__button .ck.ck-input-color__button__preview>.ck.ck-input-color__button__preview__no-color-indicator {
    display: block;
    position: absolute;
    }

    [dir='ltr'] .ck.ck-input-color>.ck.ck-input-text {
    border-bottom-right-radius: 0;
    border-top-right-radius: 0;
    }

    [dir='rtl'] .ck.ck-input-color>.ck.ck-input-text {
    border-bottom-left-radius: 0;
    border-top-left-radius: 0;
    }

    .ck.ck-input-color>.ck.ck-input-text:focus {
    z-index: 0;
    }

    .ck.ck-input-color>.ck.ck-dropdown>.ck.ck-button.ck-input-color__button {
    padding: 0;
    }

    [dir='ltr'] .ck.ck-input-color>.ck.ck-dropdown>.ck.ck-button.ck-input-color__button {
    border-bottom-left-radius: 0;
    border-top-left-radius: 0;
    }

    [dir='ltr'] .ck.ck-input-color>.ck.ck-dropdown>.ck.ck-button.ck-input-color__button:not(:focus) {
    border-left: 1px solid transparent;
    }

    [dir='rtl'] .ck.ck-input-color>.ck.ck-dropdown>.ck.ck-button.ck-input-color__button {
    border-bottom-right-radius: 0;
    border-top-right-radius: 0;
    }

    [dir='rtl'] .ck.ck-input-color>.ck.ck-dropdown>.ck.ck-button.ck-input-color__button:not(:focus) {
    border-right: 1px solid transparent;
    }

    .ck.ck-input-color>.ck.ck-dropdown>.ck.ck-button.ck-input-color__button.ck-disabled {
    background: var(--ck-color-input-disabled-background);
    }

    .ck.ck-input-color>.ck.ck-dropdown>.ck.ck-button.ck-input-color__button>.ck.ck-input-color__button__preview {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-input-color>.ck.ck-dropdown>.ck.ck-button.ck-input-color__button>.ck.ck-input-color__button__preview,
    .ck.ck-input-color>.ck.ck-dropdown>.ck.ck-button.ck-input-color__button>.ck.ck-input-color__button__preview.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    }

    .ck.ck-input-color>.ck.ck-dropdown>.ck.ck-button.ck-input-color__button>.ck.ck-input-color__button__preview {
    border: 1px solid var(--ck-color-input-border);
    height: 20px;
    width: 20px;
    }

    .ck.ck-input-color>.ck.ck-dropdown>.ck.ck-button.ck-input-color__button>.ck.ck-input-color__button__preview>.ck.ck-input-color__button__preview__no-color-indicator {
    background: red;
    border-radius: 2px;
    height: 150%;
    left: 50%;
    top: -30%;
    transform: rotate(45deg);
    transform-origin: 50%;
    width: 8%;
    }

    .ck.ck-input-color .ck.ck-input-color__remove-color {
    border-bottom-left-radius: 0;
    border-bottom-right-radius: 0;
    padding: calc(var(--ck-spacing-standard) / 2) var(--ck-spacing-standard);
    width: 100%;
    }

    .ck.ck-input-color .ck.ck-input-color__remove-color:not(:focus) {
    border-bottom: 1px solid var(--ck-color-input-border);
    }

    [dir='ltr'] .ck.ck-input-color .ck.ck-input-color__remove-color {
    border-top-right-radius: 0;
    }

    [dir='rtl'] .ck.ck-input-color .ck.ck-input-color__remove-color {
    border-top-left-radius: 0;
    }

    .ck.ck-input-color .ck.ck-input-color__remove-color .ck.ck-icon {
    margin-right: var(--ck-spacing-standard);
    }

    [dir='rtl'] .ck.ck-input-color .ck.ck-input-color__remove-color .ck.ck-icon {
    margin-left: var(--ck-spacing-standard);
    margin-right: 0;
    }

    .ck.ck-form__row {
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-between;
    }

    .ck.ck-form__row> :not(.ck-label) {
    flex-grow: 1;
    }

    .ck.ck-form__row.ck-table-form__action-row .ck-button-cancel,
    .ck.ck-form__row.ck-table-form__action-row .ck-button-save {
    justify-content: center;
    }

    .ck.ck-form__row {
    padding: var(--ck-spacing-standard) var(--ck-spacing-large) 0;
    }

    [dir='ltr'] .ck.ck-form__row> :not(.ck-label)+* {
    margin-left: var(--ck-spacing-large);
    }

    [dir='rtl'] .ck.ck-form__row> :not(.ck-label)+* {
    margin-right: var(--ck-spacing-large);
    }

    .ck.ck-form__row>.ck-label {
    min-width: 100%;
    width: 100%;
    }

    .ck.ck-form__row.ck-table-form__action-row {
    margin-top: var(--ck-spacing-large);
    }

    .ck.ck-form__row.ck-table-form__action-row .ck-button .ck-button__label {
    color: var(--ck-color-text);
    }

    .ck.ck-form {
    padding: 0 0 var(--ck-spacing-large);
    }

    .ck.ck-form:focus {
    outline: none;
    }

    .ck.ck-form .ck.ck-input-text {
    min-width: 100%;
    width: 0;
    }

    .ck.ck-form .ck.ck-dropdown {
    min-width: 100%;
    }

    .ck.ck-form .ck.ck-dropdown .ck-dropdown__button:not(:focus) {
    border: 1px solid var(--ck-color-base-border);
    }

    .ck.ck-form .ck.ck-dropdown .ck-dropdown__button .ck-button__label {
    width: 100%;
    }

    .ck.ck-table-form .ck-form__row.ck-table-form__background-row,
    .ck.ck-table-form .ck-form__row.ck-table-form__border-row {
    flex-wrap: wrap;
    }

    .ck.ck-table-form .ck-form__row.ck-table-form__dimensions-row {
    align-items: center;
    flex-wrap: wrap;
    }

    .ck.ck-table-form .ck-form__row.ck-table-form__dimensions-row .ck-labeled-field-view {
    align-items: center;
    display: flex;
    flex-direction: column-reverse;
    }

    .ck.ck-table-form .ck-form__row.ck-table-form__dimensions-row .ck-labeled-field-view .ck.ck-dropdown,
    .ck.ck-table-form .ck-form__row.ck-table-form__dimensions-row .ck-table-form__dimension-operator {
    flex-grow: 0;
    }

    .ck.ck-table-form .ck.ck-labeled-field-view {
    position: relative;
    }

    .ck.ck-table-form .ck.ck-labeled-field-view .ck.ck-labeled-field-view__status {
    bottom: calc(var(--ck-table-properties-error-arrow-size) * -1);
    left: 50%;
    position: absolute;
    transform: translate(-50%, 100%);
    z-index: 1;
    }

    .ck.ck-table-form .ck.ck-labeled-field-view .ck.ck-labeled-field-view__status:after {
    content: '';
    left: 50%;
    position: absolute;
    top: calc(var(--ck-table-properties-error-arrow-size) * -1);
    transform: translateX(-50%);
    }

    :root {
    --ck-table-properties-error-arrow-size: 6px;
    --ck-table-properties-min-error-width: 150px;
    }

    .ck.ck-table-form .ck-form__row.ck-table-form__border-row .ck-labeled-field-view>.ck-label {
    font-size: var(--ck-font-size-tiny);
    text-align: center;
    }

    .ck.ck-table-form .ck-form__row.ck-table-form__border-row .ck-table-form__border-style,
    .ck.ck-table-form .ck-form__row.ck-table-form__border-row .ck-table-form__border-width {
    max-width: 80px;
    min-width: 80px;
    width: 80px;
    }

    .ck.ck-table-form .ck-form__row.ck-table-form__dimensions-row {
    padding: 0;
    }

    .ck.ck-table-form .ck-form__row.ck-table-form__dimensions-row .ck-table-form__dimensions-row__height,
    .ck.ck-table-form .ck-form__row.ck-table-form__dimensions-row .ck-table-form__dimensions-row__width {
    margin: 0;
    }

    .ck.ck-table-form .ck-form__row.ck-table-form__dimensions-row .ck-table-form__dimension-operator {
    align-self: flex-end;
    display: inline-block;
    height: var(--ck-ui-component-min-height);
    line-height: var(--ck-ui-component-min-height);
    margin: 0 var(--ck-spacing-small);
    }

    .ck.ck-table-form .ck.ck-labeled-field-view {
    padding-top: var(--ck-spacing-standard);
    }

    .ck.ck-table-form .ck.ck-labeled-field-view .ck.ck-labeled-field-view__status {
    border-radius: 0;
    }

    .ck-rounded-corners .ck.ck-table-form .ck.ck-labeled-field-view .ck.ck-labeled-field-view__status,
    .ck.ck-table-form .ck.ck-labeled-field-view .ck.ck-labeled-field-view__status.ck-rounded-corners {
    border-radius: var(--ck-border-radius);
    }

    .ck.ck-table-form .ck.ck-labeled-field-view .ck.ck-labeled-field-view__status {
    background: var(--ck-color-base-error);
    color: var(--ck-color-base-background);
    min-width: var(--ck-table-properties-min-error-width);
    padding: var(--ck-spacing-small) var(--ck-spacing-medium);
    text-align: center;
    }

    .ck.ck-table-form .ck.ck-labeled-field-view .ck.ck-labeled-field-view__status:after {
    border-color: transparent transparent var(--ck-color-base-error) transparent;
    border-style: solid;
    border-width: 0 var(--ck-table-properties-error-arrow-size) var(--ck-table-properties-error-arrow-size) var(--ck-table-properties-error-arrow-size);
    }

    .ck.ck-table-form .ck.ck-labeled-field-view .ck.ck-labeled-field-view__status {
    animation: ck-table-form-labeled-view-status-appear 0.15s ease both;
    }

    .ck.ck-table-form .ck.ck-labeled-field-view .ck-input.ck-error:not(:focus)+.ck.ck-labeled-field-view__status {
    display: none;
    }

    @keyframes ck-table-form-labeled-view-status-appear {
    0% {
        opacity: 0;
    }

    to {
        opacity: 1;
    }
    }

    .ck.ck-table-cell-properties-form .ck-form__row.ck-table-cell-properties-form__alignment-row {
    flex-wrap: wrap;
    }

    .ck.ck-table-cell-properties-form .ck-form__row.ck-table-cell-properties-form__alignment-row .ck.ck-toolbar:first-of-type {
    flex-grow: 0.57;
    }

    .ck.ck-table-cell-properties-form .ck-form__row.ck-table-cell-properties-form__alignment-row .ck.ck-toolbar:last-of-type {
    flex-grow: 0.43;
    }

    .ck.ck-table-cell-properties-form .ck-form__row.ck-table-cell-properties-form__alignment-row .ck.ck-toolbar .ck-button {
    flex-grow: 1;
    }

    .ck.ck-table-cell-properties-form {
    width: 320px;
    }

    .ck.ck-table-cell-properties-form .ck-form__row.ck-table-cell-properties-form__padding-row {
    align-self: flex-end;
    padding: 0;
    width: 25%;
    }

    .ck.ck-table-cell-properties-form .ck-form__row.ck-table-cell-properties-form__alignment-row .ck.ck-toolbar {
    background: none;
    margin-top: var(--ck-spacing-standard);
    }

    .ck.ck-table-properties-form .ck-form__row.ck-table-properties-form__alignment-row {
    align-content: baseline;
    flex-basis: 0;
    flex-wrap: wrap;
    }

    .ck.ck-table-properties-form .ck-form__row.ck-table-properties-form__alignment-row .ck.ck-toolbar .ck-toolbar__items {
    flex-wrap: nowrap;
    }

    .ck.ck-table-properties-form {
    width: 320px;
    }

    .ck.ck-table-properties-form .ck-form__row.ck-table-properties-form__alignment-row {
    align-self: flex-end;
    padding: 0;
    }

    .ck.ck-table-properties-form .ck-form__row.ck-table-properties-form__alignment-row .ck.ck-toolbar {
    background: none;
    margin-top: var(--ck-spacing-standard);
    }

    .ck.ck-table-properties-form .ck-form__row.ck-table-properties-form__alignment-row .ck.ck-toolbar .ck-toolbar__items>* {
    width: 40px;
    }

    :root {
    --ck-color-selector-caption-background: #f7f7f7;
    --ck-color-selector-caption-text: #333;
    --ck-color-selector-caption-highlighted-background: #fd0;
    }

    .ck-content .table>figcaption {
    background-color: var(--ck-color-selector-caption-background);
    caption-side: top;
    color: var(--ck-color-selector-caption-text);
    display: table-caption;
    font-size: 0.75em;
    outline-offset: -1px;
    padding: 0.6em;
    text-align: center;
    word-break: break-word;
    }

    .ck.ck-editor__editable .table>figcaption.table__caption_highlighted {
    animation: ck-table-caption-highlight 0.6s ease-out;
    }

    .ck.ck-editor__editable .table>figcaption.ck-placeholder:before {
    overflow: hidden;
    padding-left: inherit;
    padding-right: inherit;
    text-overflow: ellipsis;
    white-space: nowrap;
    }

    @keyframes ck-table-caption-highlight {
    0% {
        background-color: var(--ck-color-selector-caption-highlighted-background);
    }

    to {
        background-color: var(--ck-color-selector-caption-background);
    }
    }

    :root {
    --ck-color-selector-column-resizer-hover: var(--ck-color-base-active);
    --ck-table-column-resizer-width: 7px;
    --ck-table-column-resizer-position-offset: calc(var(--ck-table-column-resizer-width) * -0.5 - 0.5px);
    }

    .ck-content .table .ck-table-resized {
    table-layout: fixed;
    }

    .ck-content .table table {
    overflow: hidden;
    }

    .ck-content .table td,
    .ck-content .table th {
    overflow-wrap: break-word;
    position: relative;
    }

    .ck.ck-editor__editable .table .ck-table-column-resizer {
    bottom: 0;
    cursor: col-resize;
    position: absolute;
    right: var(--ck-table-column-resizer-position-offset);
    top: 0;
    user-select: none;
    width: var(--ck-table-column-resizer-width);
    z-index: var(--ck-z-default);
    }

    .ck.ck-editor__editable .table[draggable] .ck-table-column-resizer,
    .ck.ck-editor__editable.ck-column-resize_disabled .table .ck-table-column-resizer {
    display: none;
    }

    .ck.ck-editor__editable .table .ck-table-column-resizer:hover,
    .ck.ck-editor__editable .table .ck-table-column-resizer__active {
    background-color: var(--ck-color-selector-column-resizer-hover);
    bottom: -999999px;
    opacity: 0.25;
    top: -999999px;
    }

    .ck.ck-editor__editable[dir='rtl'] .table .ck-table-column-resizer {
    left: var(--ck-table-column-resizer-position-offset);
    right: unset;
    }</style>

```
    
## Documentation

[Ckeditor5](https://ckeditor.com/docs/ckeditor5/latest/installation/integrations/vuejs-v3.html)

