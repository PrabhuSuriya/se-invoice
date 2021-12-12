<script>
  const print = () => {
    window.print();
  }
</script>

<header class="d-flex justify-content-center" style="text-align: center;">
  <h4>Tax Invoice</h4>
  <button on:click={print} class="btn btn-print no-print" role="button">Print</button>
</header>
<main class="flex">
  <div class="sample-watermark">Sample For Review</div>
  <section class="form-container d-flex">
      <section class="invoice">
          <section class="content flex">
              <div class="flex flex-c" style="min-height: 3in; flex-grow: 1; width: 50%;">
                  <div class="flex  bb br  flex-c" style="height: 50%;">
                      <div class="label" style="line-height: 1.5; font-size: 1rem;">
                          <pre>
Scientific & Elextric Co.
No: 153/76, Thambu Chetty Street,
Chennai 600001
Phone: 9999911111
GCTIN/UIN : 0000XXXXXXXXXX
State Name : Tamil Nadu, Code: 33


                        </pre>
                      </div>
                  </div>
                  <div class="flex br bb  flex-c" style="height: 50%;">
                      <div class="label" style="flex-grow: 1">Name</div>
                      <div contenteditable="true" class="value" style="flex-grow: 7" />
                  </div>
              </div>
              
              <div class="flex flex-c"style="min-height: 3in; flex-grow: 1; width: 50%;">

                <div class="flex  " >
                    <div class="flex   flex-c" style="min-height: 3in; flex-grow: 1; width: 50%;">
                        <div class="flex br bb  flex-c" style="min-height: 0.4in; flex-grow: 1;">
                            <div class="label">Name</div>
                            <div contenteditable="true" class="value" />
                        </div>
                        <div class="flex br bb  flex-c" style="min-height: 0.4in; flex-grow: 1;">
                            <div class="label">Name</div>
                            <div contenteditable="true" class="value" />
                        </div>
                        <div class="flex br bb  flex-c" style="min-height: 0.4in; flex-grow: 1;">
                            <div class="label">Name</div>
                            <div contenteditable="true" class="value" />
                        </div>
                        <div class="flex br bb  flex-c" style="min-height: 0.4in; flex-grow: 1;">
                            <div class="label">Name</div>
                            <div contenteditable="true" class="value" />
                        </div>
                        <div class="flex br bb  flex-c" style="min-height: 0.4in; flex-grow: 1;">
                            <div class="label">Name</div>
                            <div contenteditable="true" class="value" />
                        </div>
                        <div class="flex br bb  flex-c" style="min-height: 0.4in; flex-grow: 1;">
                            <div class="label">Name</div>
                            <div contenteditable="true" class="value" />
                        </div>
                    </div>
                    <div class="flex   flex-c" style="min-height: 3in; flex-grow: 1; width: 50%;">
                      <div class="flex  bb  flex-c" style="min-height: 0.4in; flex-grow: 1;">
                          <div class="label">Name</div>
                          <div contenteditable="true" class="value" />
                      </div>
                      <div class="flex  bb  flex-c" style="min-height: 0.4in; flex-grow: 1;">
                          <div class="label">Name</div>
                          <div contenteditable="true" class="value" />
                      </div>
                      <div class="flex  bb  flex-c" style="min-height: 0.4in; flex-grow: 1;">
                          <div class="label">Name</div>
                          <div contenteditable="true" class="value" />
                      </div>
                      <div class="flex  bb  flex-c" style="min-height: 0.4in; flex-grow: 1;">
                          <div class="label">Name</div>
                          <div contenteditable="true" class="value" />
                      </div>
                      <div class="flex  bb  flex-c" style="min-height: 0.4in; flex-grow: 1;">
                          <div class="label">Name</div>
                          <div contenteditable="true" class="value" />
                      </div>
                      <div class="flex  bb  flex-c" style="min-height: 0.4in; flex-grow: 1;">
                          <div class="label">Name</div>
                          <div contenteditable="true" class="value" />
                      </div>
                  </div>
                </div>
                <div class="flex" >
                  <div class="flex bb  flex-c" style="min-height: 0.6in; flex-grow: 2;">
                      <div class="label">Delivery Instructions</div>
                      <div contenteditable="true" class="value" />
                  </div>
                </div>
              </div>
              
          </section>
      </section>
  </section>
</main>


<style lang="scss">
  .invoice {
    height: 10.5in;
    width: 7.8in;
    border: 1px solid gray;
    margin: 0 auto;
    .flex {
      display: flex;
    }
    .flex-c {
      flex-direction: column;
    }
    .s-border {
      border: 1px solid gray;
      border-width: 0 1px 1px 0;
    }
    * {
      border-width: 0;
    }
    .bt {
      border-top: 1px solid gray !important;
    }
    .br {
      border-right: 1px solid gray !important;
    }
    .bb {
      border-bottom: 1px solid gray !important;
    }
    .bl {
      border-left: 1px solid gray !important;
    }
    .label {
      flex-grow: 1;
      text-align: left;
      padding-left: 5px;
      font-weight: bold;
      font-size: 0.8rem;
      display: flex;
      align-items: center;
    }
    .value {
      font-size: .9rem;
      flex-grow: 3;
      text-align: left;
      padding-left: 8px;
      &[contenteditable="true"]:focus {
        background-color: rgba(217, 245, 255, 0.5);
        line-height: 1;
        outline: none;
        font-size: 1rem;
        display: inline-block;
      }
    }
    // .content {
    //   border: 1px solid gray;
    //   // margin: .5in;
    //   height: -webkit-fill-available;

    // }
  }
  /* .container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 2em 2em 2em 2em 2em;
  gap: 0px 0px;
  grid-auto-flow: row;
  grid-template-areas:
    ". ."
    ". ."
    ". ."
    ". ."
    ". .";
} */

  /* CSS */
  .btn {
    background-image: linear-gradient(#42a1ec, #0070c9);
    border: 1px solid #0077cc;
    border-radius: 4px;
    box-sizing: border-box;
    color: #ffffff;
    cursor: pointer;
    direction: ltr;
    display: block;
    font-family: "SF Pro Text", "SF Pro Icons", "AOS Icons", "Helvetica Neue",
      Helvetica, Arial, sans-serif;
    font-size: 17px;
    font-weight: 400;
    letter-spacing: -0.022em;
    line-height: 1.47059;
    min-width: 30px;
    overflow: visible;
    padding: 4px 15px;
    text-align: center;
    vertical-align: baseline;
    user-select: none;
    -webkit-user-select: none;
    touch-action: manipulation;
    white-space: nowrap;
  }

  .btn:disabled {
    cursor: default;
    opacity: 0.3;
  }

  .btn:hover {
    background-image: linear-gradient(#51a9ee, #147bcd);
    border-color: #1482d0;
    text-decoration: none;
  }

  .btn:active {
    background-image: linear-gradient(#3d94d9, #0067b9);
    border-color: #006dbc;
    outline: none;
  }

  .btn:focus {
    box-shadow: rgba(131, 192, 253, 0.5) 0 0 0 3px;
    outline: none;
  }
  .btn-print{
    position: fixed;
    right: 1rem;
    top: 1rem;
  }
  .no-print {
    @media print {
      display: none;
    }
  }
  .sample-watermark {
    position: fixed;
    top: 50%;
    left: 50%;
    font-size: 5rem;
    font-weight: 800;
    opacity: 0.2;
    white-space: nowrap;
    transform: translateX(-50%) translateY(-50%) rotate(
314deg);
  }
  main {
    text-align: center;
    padding: 1em;
    /* max-width: 240px; */
    margin: 0 auto;
    // align-items: center;
    // justify-content: center;
  }
  /* 
  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  table {
    width: 100%;
    border-collapse: collapse;
    border: 1px solid gray;
  }
  td,
  th {
    border: 1px solid gray;
  } */
</style>
