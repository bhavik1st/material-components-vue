<template>
    <m-layout-grid-inner>
         <m-layout-grid-cell :span="12">
            <m-typo-display :level="1">Button</m-typo-display>
            <m-typo-body :level="2">
                <a href="https://github.com/matsp/material-components-vue/blob/master/components/Button">
                    https://github.com/matsp/material-components-vue/blob/master/components/Button
                </a>
            </m-typo-body>
         </m-layout-grid-cell>
        <m-layout-grid-cell :span="12">
            <m-typo-headline>Text</m-typo-headline>
            <m-layout-grid-inner>
                <m-layout-grid-cell :span="3">
                    <m-button>text</m-button>
                </m-layout-grid-cell>
                <m-layout-grid-cell :span="3">
                    <m-button interactive>interactive</m-button>
                </m-layout-grid-cell>
                <m-layout-grid-cell :span="3">
                    <m-button icon="cloud">icon</m-button>
                </m-layout-grid-cell>
                <m-layout-grid-cell :span="3">
                    <m-button compact>compact</m-button>
                </m-layout-grid-cell>
                <m-layout-grid-cell :span="3">
                    <m-button dense>dense</m-button>
                </m-layout-grid-cell>
                <m-layout-grid-cell :span="3">
                    <m-button disabled>disabled</m-button>
                </m-layout-grid-cell>
            </m-layout-grid-inner>
        </m-layout-grid-cell>
        <m-layout-grid-cell :span="12">
            <m-typo-headline>Raised</m-typo-headline>
            <m-layout-grid-inner>
             <m-layout-grid-cell :span="3">
            <m-button raised>text</m-button>
             </m-layout-grid-cell>
              <m-layout-grid-cell :span="3">
            <m-button raised interactive>interactive</m-button>
             </m-layout-grid-cell>
             <m-layout-grid-cell :span="3">
            <m-button raised icon="cloud">icon</m-button>
             </m-layout-grid-cell>
             <m-layout-grid-cell :span="3">
            <m-button raised compact>compact</m-button>
                </m-layout-grid-cell>
            <m-layout-grid-cell :span="3">
              <m-button raised dense>dense</m-button>
            </m-layout-grid-cell>
            <m-layout-grid-cell :span="3">
              <m-button raised disabled>disabled</m-button>
            </m-layout-grid-cell>
            </m-layout-grid-inner>
        </m-layout-grid-cell>
        <m-layout-grid-cell :span="12">
            <m-typo-headline>Unelevated</m-typo-headline>
            <m-layout-grid-inner>
             <m-layout-grid-cell :span="3">
            <m-button unelevated>text</m-button>
             </m-layout-grid-cell>
              <m-layout-grid-cell :span="3">
            <m-button unelevated interactive>interactive</m-button>
             </m-layout-grid-cell>
             <m-layout-grid-cell :span="3">
            <m-button unelevated icon="cloud">icon</m-button>
             </m-layout-grid-cell>
             <m-layout-grid-cell :span="3">
            <m-button unelevated compact>compact</m-button>
                </m-layout-grid-cell>
            <m-layout-grid-cell :span="3">
              <m-button unelevated dense>dense</m-button>
            </m-layout-grid-cell>
            <m-layout-grid-cell :span="3">
              <m-button unelevated disabled>disabled</m-button>
            </m-layout-grid-cell>
            </m-layout-grid-inner>
        </m-layout-grid-cell>
        <m-layout-grid-cell :span="12">
            <m-typo-headline>Stroked</m-typo-headline>
            <m-layout-grid-inner>
             <m-layout-grid-cell :span="3">
            <m-button stroked>text</m-button>
             </m-layout-grid-cell>
              <m-layout-grid-cell :span="3">
            <m-button stroked interactive>interactive</m-button>
             </m-layout-grid-cell>
             <m-layout-grid-cell :span="3">
            <m-button stroked icon="cloud">icon</m-button>
             </m-layout-grid-cell>
             <m-layout-grid-cell :span="3">
            <m-button stroked compact>compact</m-button>
                </m-layout-grid-cell>
            <m-layout-grid-cell :span="3">
              <m-button stroked dense>dense</m-button>
            </m-layout-grid-cell>
            <m-layout-grid-cell :span="3">
              <m-button stroked disabled>disabled</m-button>
            </m-layout-grid-cell>
            </m-layout-grid-inner>
        </m-layout-grid-cell>
    </m-layout-grid-inner>
</template>
