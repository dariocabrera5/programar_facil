<template>
    <class>{{drawflow}}</class>
</template>
<script>
export default {
data(){
    return{
    "drawflow": {
        "Home": {
            "data": {
                "4": {
                    "id": 4,
                    "name": "email",
                    "data": {},
                    "class": "email",
                    "html": "\n\n   Send Email \n\n",
                    "typenode": false,
                    "inputs": {
                        "input_1": {
                            "connections": [
                                {
                                    "node": "5",
                                    "input": "output_1"
                                }
                            ]
                        }
                    },
                    "outputs": {},
                    "pos_x": 638.4285714285714,
                    "pos_y": 22
                },
                "5": {
                    "id": 5,
                    "name": "template",
                    "data": {
                        "template": "Write your template"
                    },
                    "class": "template",
                    "html": "\n \n Template\n \nGer Vars\n\nOutput template with vars\n\n\n",
                    "typenode": false,
                    "inputs": {
                        "input_1": {
                            "connections": []
                        }
                    },
                    "outputs": {
                        "output_1": {
                            "connections": [
                                {
                                    "node": "4",
                                    "output": "input_1"
                                },
                                {
                                    "node": "11",
                                    "output": "input_1"
                                }
                            ]
                        }
                    },
                    "pos_x": 161,
                    "pos_y": 74.42857142857143
                },
                "11": {
                    "id": 11,
                    "name": "log",
                    "data": {},
                    "class": "log",
                    "html": "\n\nSave log file \n\n",
                    "typenode": false,
                    "inputs": {
                        "input_1": {
                            "connections": [
                                {
                                    "node": "5",
                                    "input": "output_1"
                                }
                            ]
                        }
                    },
                    "outputs": {},
                    "pos_x": 692.4285714285714,
                    "pos_y": 297.57142857142856
                }
            }
        },
        "Other": {
            "data": {
                "8": {
                    "id": 8,
                    "name": "personalized",
                    "data": {},
                    "class": "personalized",
                    "html": "\n\nPersonalized\n\n",
                    "typenode": false,
                    "inputs": {
                        "input_1": {
                            "connections": [
                                {
                                    "node": "12",
                                    "input": "output_1"
                                },
                                {
                                    "node": "12",
                                    "input": "output_2"
                                },
                                {
                                    "node": "12",
                                    "input": "output_3"
                                },
                                {
                                    "node": "12",
                                    "input": "output_4"
                                }
                            ]
                        }
                    },
                    "outputs": {
                        "output_1": {
                            "connections": [
                                {
                                    "node": "9",
                                    "output": "input_1"
                                }
                            ]
                        }
                    },
                    "pos_x": 764,
                    "pos_y": 227
                },
                "9": {
                    "id": 9,
                    "name": "dbclick",
                    "data": {
                        "name": "Hello World!!"
                    },
                    "class": "dbclick",
                    "html": "\n\nDb Click\n\nDb Click here\n\n\n×\nChange your variable {name} !\n\n\n\n\n\n\n",
                    "typenode": false,
                    "inputs": {
                        "input_1": {
                            "connections": [
                                {
                                    "node": "8",
                                    "input": "output_1"
                                }
                            ]
                        }
                    },
                    "outputs": {
                        "output_1": {
                            "connections": [
                                {
                                    "node": "12",
                                    "output": "input_2"
                                }
                            ]
                        }
                    },
                    "pos_x": 209,
                    "pos_y": 38
                },
                "12": {
                    "id": 12,
                    "name": "multiple",
                    "data": {},
                    "class": "multiple",
                    "html": "\n\n\nMultiple!\n\n\n",
                    "typenode": false,
                    "inputs": {
                        "input_1": {
                            "connections": []
                        },
                        "input_2": {
                            "connections": [
                                {
                                    "node": "9",
                                    "input": "output_1"
                                }
                            ]
                        },
                        "input_3": {
                            "connections": []
                        }
                    },
                    "outputs": {
                        "output_1": {
                            "connections": [
                                {
                                    "node": "8",
                                    "output": "input_1"
                                }
                            ]
                        },
                        "output_2": {
                            "connections": [
                                {
                                    "node": "8",
                                    "output": "input_1"
                                }
                            ]
                        },
                        "output_3": {
                            "connections": [
                                {
                                    "node": "8",
                                    "output": "input_1"
                                }
                            ]
                        },
                        "output_4": {
                            "connections": [
                                {
                                    "node": "8",
                                    "output": "input_1"
                                }
                            ]
                        }
                    },
                    "pos_x": 177,
                    "pos_y": 272
                }
            }
        }
    }
}

    }
}

</script>
<style scoped>
:root {
  --dfBackgroundColor: #ffffff;
  --dfBackgroundSize: 0px;
  --dfBackgroundImage: none;

  --dfNodeType: flex;
  --dfNodeTypeFloat: none;
  --dfNodeBackgroundColor: #ffffff;
  --dfNodeTextColor: #000000;
  --dfNodeBorderSize: 2px;
  --dfNodeBorderColor: #000000;
  --dfNodeBorderRadius: 4px;
  --dfNodeMinHeight: 40px;
  --dfNodeMinWidth: 160px;
  --dfNodePaddingTop: 15px;
  --dfNodePaddingBottom: 15px;
  --dfNodeBoxShadowHL: 0px;
  --dfNodeBoxShadowVL: 2px;
  --dfNodeBoxShadowBR: 15px;
  --dfNodeBoxShadowS: 2px;
  --dfNodeBoxShadowColor: #000000;

  --dfNodeHoverBackgroundColor: #ffffff;
  --dfNodeHoverTextColor: #000000;
  --dfNodeHoverBorderSize: 2px;
  --dfNodeHoverBorderColor: #000000;
  --dfNodeHoverBorderRadius: 4px;

  --dfNodeHoverBoxShadowHL: 0px;
  --dfNodeHoverBoxShadowVL: 2px;
  --dfNodeHoverBoxShadowBR: 15px;
  --dfNodeHoverBoxShadowS: 2px;
  --dfNodeHoverBoxShadowColor: #4ea9ff;

  --dfNodeSelectedBackgroundColor: #000000;
  --dfNodeSelectedTextColor: #ffffff;
  --dfNodeSelectedBorderSize: 2px;
  --dfNodeSelectedBorderColor: #000000;
  --dfNodeSelectedBorderRadius: 4px;

  --dfNodeSelectedBoxShadowHL: 0px;
  --dfNodeSelectedBoxShadowVL: 2px;
  --dfNodeSelectedBoxShadowBR: 15px;
  --dfNodeSelectedBoxShadowS: 2px;
  --dfNodeSelectedBoxShadowColor: #4ea9ff;

  --dfInputBackgroundColor: #ffffff;
  --dfInputBorderSize: 2px;
  --dfInputBorderColor: #000000;
  --dfInputBorderRadius: 50px;
  --dfInputLeft: -27px;
  --dfInputHeight: 20px;
  --dfInputWidth: 20px;

  --dfInputHoverBackgroundColor: #ffffff;
  --dfInputHoverBorderSize: 2px;
  --dfInputHoverBorderColor: #000000;
  --dfInputHoverBorderRadius: 50px;

  --dfOutputBackgroundColor: #ffffff;
  --dfOutputBorderSize: 2px;
  --dfOutputBorderColor: #000000;
  --dfOutputBorderRadius: 50px;
  --dfOutputRight: -3px;
  --dfOutputHeight: 20px;
  --dfOutputWidth: 20px;

  --dfOutputHoverBackgroundColor: #ffffff;
  --dfOutputHoverBorderSize: 2px;
  --dfOutputHoverBorderColor: #000000;
  --dfOutputHoverBorderRadius: 50px;

  --dfLineWidth: 5px;
  --dfLineColor: #4682b4;
  --dfLineHoverColor: #4682b4;
  --dfLineSelectedColor: #43b993;

  --dfRerouteBorderWidth: 2px;
  --dfRerouteBorderColor: #000000;
  --dfRerouteBackgroundColor: #ffffff;

  --dfRerouteHoverBorderWidth: 2px;
  --dfRerouteHoverBorderColor: #000000;
  --dfRerouteHoverBackgroundColor: #ffffff;

  --dfDeleteDisplay: block;
  --dfDeleteColor: #ffffff;
  --dfDeleteBackgroundColor: #000000;
  --dfDeleteBorderSize: 2px;
  --dfDeleteBorderColor: #ffffff;
  --dfDeleteBorderRadius: 50px;
  --dfDeleteTop: -15px;

  --dfDeleteHoverColor: #000000;
  --dfDeleteHoverBackgroundColor: #ffffff;
  --dfDeleteHoverBorderSize: 2px;
  --dfDeleteHoverBorderColor: #000000;
  --dfDeleteHoverBorderRadius: 50px;

}

#drawflow {
  background: var(--dfBackgroundColor);
  background-size: var(--dfBackgroundSize) var(--dfBackgroundSize);
  background-image: var(--dfBackgroundImage);
}

.drawflow .drawflow-node {
  display: var(--dfNodeType);
  background: var(--dfNodeBackgroundColor);
  color: var(--dfNodeTextColor);
  border: var(--dfNodeBorderSize)  solid var(--dfNodeBorderColor);
  border-radius: var(--dfNodeBorderRadius);
  min-height: var(--dfNodeMinHeight);
  width: auto;
  min-width: var(--dfNodeMinWidth);
  padding-top: var(--dfNodePaddingTop);
  padding-bottom: var(--dfNodePaddingBottom);
  -webkit-box-shadow: var(--dfNodeBoxShadowHL) var(--dfNodeBoxShadowVL) var(--dfNodeBoxShadowBR) var(--dfNodeBoxShadowS) var(--dfNodeBoxShadowColor);
  box-shadow:  var(--dfNodeBoxShadowHL) var(--dfNodeBoxShadowVL) var(--dfNodeBoxShadowBR) var(--dfNodeBoxShadowS) var(--dfNodeBoxShadowColor);
}

.drawflow .drawflow-node:hover {
  background: var(--dfNodeHoverBackgroundColor);
  color: var(--dfNodeHoverTextColor);
  border: var(--dfNodeHoverBorderSize)  solid var(--dfNodeHoverBorderColor);
  border-radius: var(--dfNodeHoverBorderRadius);
  -webkit-box-shadow: var(--dfNodeHoverBoxShadowHL) var(--dfNodeHoverBoxShadowVL) var(--dfNodeHoverBoxShadowBR) var(--dfNodeHoverBoxShadowS) var(--dfNodeHoverBoxShadowColor);
  box-shadow:  var(--dfNodeHoverBoxShadowHL) var(--dfNodeHoverBoxShadowVL) var(--dfNodeHoverBoxShadowBR) var(--dfNodeHoverBoxShadowS) var(--dfNodeHoverBoxShadowColor);
}

.drawflow .drawflow-node.selected {
  background: var(--dfNodeSelectedBackgroundColor);
  color: var(--dfNodeSelectedTextColor);
  border: var(--dfNodeSelectedBorderSize)  solid var(--dfNodeSelectedBorderColor);
  border-radius: var(--dfNodeSelectedBorderRadius);
  -webkit-box-shadow: var(--dfNodeSelectedBoxShadowHL) var(--dfNodeSelectedBoxShadowVL) var(--dfNodeSelectedBoxShadowBR) var(--dfNodeSelectedBoxShadowS) var(--dfNodeSelectedBoxShadowColor);
  box-shadow:  var(--dfNodeSelectedBoxShadowHL) var(--dfNodeSelectedBoxShadowVL) var(--dfNodeSelectedBoxShadowBR) var(--dfNodeSelectedBoxShadowS) var(--dfNodeSelectedBoxShadowColor);
}

.drawflow .drawflow-node .input {
  left: var(--dfInputLeft);
  background: var(--dfInputBackgroundColor);
  border: var(--dfInputBorderSize)  solid var(--dfInputBorderColor);
  border-radius: var(--dfInputBorderRadius);
  height: var(--dfInputHeight);
  width: var(--dfInputWidth);
}

.drawflow .drawflow-node .input:hover {
  background: var(--dfInputHoverBackgroundColor);
  border: var(--dfInputHoverBorderSize)  solid var(--dfInputHoverBorderColor);
  border-radius: var(--dfInputHoverBorderRadius);
}

.drawflow .drawflow-node .outputs {
  float: var(--dfNodeTypeFloat);
}

.drawflow .drawflow-node .output {
  right: var(--dfOutputRight);
  background: var(--dfOutputBackgroundColor);
  border: var(--dfOutputBorderSize)  solid var(--dfOutputBorderColor);
  border-radius: var(--dfOutputBorderRadius);
  height: var(--dfOutputHeight);
  width: var(--dfOutputWidth);
}

.drawflow .drawflow-node .output:hover {
  background: var(--dfOutputHoverBackgroundColor);
  border: var(--dfOutputHoverBorderSize)  solid var(--dfOutputHoverBorderColor);
  border-radius: var(--dfOutputHoverBorderRadius);
}

.drawflow .connection .main-path {
  stroke-width: var(--dfLineWidth);
  stroke: var(--dfLineColor);
}

.drawflow .connection .main-path:hover {
  stroke: var(--dfLineHoverColor);
}

.drawflow .connection .main-path.selected {
  stroke: var(--dfLineSelectedColor);
}

.drawflow .connection .point {
  stroke: var(--dfRerouteBorderColor);
  stroke-width: var(--dfRerouteBorderWidth);
  fill: var(--dfRerouteBackgroundColor);
}

.drawflow .connection .point:hover {
  stroke: var(--dfRerouteHoverBorderColor);
  stroke-width: var(--dfRerouteHoverBorderWidth);
  fill: var(--dfRerouteHoverBackgroundColor);
}

.drawflow-delete {
  display: var(--dfDeleteDisplay);
  color: var(--dfDeleteColor);
  background: var(--dfDeleteBackgroundColor);
  border: var(--dfDeleteBorderSize) solid var(--dfDeleteBorderColor);
  border-radius: var(--dfDeleteBorderRadius);
}

.parent-node .drawflow-delete {
  top: var(--dfDeleteTop);
}

.drawflow-delete:hover {
  color: var(--dfDeleteHoverColor);
  background: var(--dfDeleteHoverBackgroundColor);
  border: var(--dfDeleteHoverBorderSize) solid var(--dfDeleteHoverBorderColor);
  border-radius: var(--dfDeleteHoverBorderRadius);
}

</style>