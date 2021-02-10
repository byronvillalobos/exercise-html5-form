<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <link
      rel="stylesheet"
      href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
      integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm"
      crossorigin="anonymous"
    />
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/css/all.min.css"
    />
  </head>

  <body>
    <div class="container">
      <div class="card mt-5">
        <div class="card-header h1">Payment for example</div>
        <form class="needs-validation p-3" novalidate>
            <div class="alert alert-danger d-block" role="alert">
                Some fields are missing
              </div>
            <div class="form-row">
            <div class="col-md-4 mb-3">
              <label for="validationCustom01">Card #</label>
              <input
                type="text"
                class="form-control"
                id="validationCustom01"
                placeholder="First name"
                value="XXXXXXXXXXXXXXXX"
                required
              />
              <div class="valid-feedback">Looks good!</div>
            </div>
            <div class="col-md-4 mb-3">
              <label for="validationCustom02">CVC #</label>
              <input
                type="text"
                class="form-control"
                id="validationCustom02"
                placeholder="Last name"
                value="0000"
                required
              />
              <div class="valid-feedback">Looks good!</div>
            </div>
            <div class="col-md-4 mb-3">
              <label for="validationCustom02">Amount</label>
              $<input
                type="text"
                class="form-control"
                id="validationCustom02"
                placeholder="Last name"
                value="Amount"
                required
              />
              <div class="valid-feedback">Looks good!</div>
            </div>
          </div>
          <div class="form-row">
            <div class="col-md-6 mb-3">
              <label for="validationCustom01">First name</label>
              <input
                type="text"
                class="form-control"
                id="validationCustom01"
                placeholder="First name"
                value=""
                required
              />
              <div class="valid-feedback">Looks good!</div>
            </div>
            <div class="col-md-6 mb-3">
              <label for="validationCustom02">Last name</label>
              <input
                type="text"
                class="form-control"
                id="validationCustom02"
                placeholder="Last name"
                value=""
                required
              />
              <div class="valid-feedback">Looks good!</div>
            </div>
          </div>
          <div class="form-row">
            <div class="col-md-6 mb-3">
              <label for="validationCustom03">City</label>
              <input
                type="text"
                class="form-control"
                id="validationCustom03"
                placeholder="City"
                required
              />
              <div class="invalid-feedback">Please provide a valid city.</div>
            </div>
            <div class="col-md-3 mb-3">
              <label for="validationCustom04">State</label>
              <select class="custom-select" id="inputGroupSelect01">
                <option selected>Pick a state</option>
                <option value="1">One</option>
                <option value="2">Two</option>
                <option value="3">Three</option>
              </select>
              <div class="invalid-feedback">Please provide a valid state.</div>
            </div>
            <div class="col-md-3 mb-3">
              <label for="validationCustom05">Postal Code</label>
              <input
                type="text"
                class="form-control"
                id="validationCustom05"
                placeholder="Zip"
                required
              />
              <div class="invalid-feedback">Please provide a valid zip.</div>
            </div>
          </div>
          <div class="form-row">
            <!-- tarjetas -->

            <div class="col-md-6">
              <label>We Accept:</label>
              <div class="w-50 bg-secondary text-white rounded p-2">
                <div class="custom-control custom-radio custom-control-inline">
                  <input
                    type="radio"
                    id="customRadioInline1"
                    name="customRadio"
                    class="custom-control-input"
                  />
                  <label class="custom-control-label" for="customRadioInline1"
                    ><i class="fab fa-cc-mastercard"></i
                  ></label>
                </div>
                <div class="custom-control custom-radio custom-control-inline">
                  <input
                    type="radio"
                    id="customRadioInline2"
                    name="customRadio"
                    class="custom-control-input"
                  />
                  <label class="custom-control-label" for="customRadioInline2"
                    ><i class="fab fa-cc-visa"></i
                  ></label>
                </div>
                <div class="custom-control custom-radio custom-control-inline">
                  <input
                    type="radio"
                    id="customRadioInline3"
                    name="customRadio"
                    class="custom-control-input"
                  />
                  <label class="custom-control-label" for="customRadioInline3"
                    ><i class="fab fa-cc-mastercard"></i
                  ></label>
                </div>
                <div class="custom-control custom-radio custom-control-inline">
                  <input
                    type="radio"
                    id="customRadioInline4"
                    name="customRadio"
                    class="custom-control-input"
                  />
                  <label class="custom-control-label" for="customRadioInline4"
                    ><i class="fab fa-cc-visa"></i
                  ></label>
                </div>
              </div>
            </div>

            <!-- Mensaje -->
            <div class="col-md-6 mb-3">
              <label for="validationCustom02">Message</label>
              <textarea
                class="form-control rounded-0"
                id="exampleFormControlTextarea1"
                rows="5"
              ></textarea>
              <p class="card-text">
                <small class="text-muted">Add any notes here.</small>
              </p>

              <div class="valid-feedback">Looks good!</div>
            </div>
          </div>

          <div class="card-footer d-flex justify-content-end">
            <button class="btn btn-secondary mr-2" type="submit">Cancel</button>
            <button class="btn btn-primary" type="submit" data-dismiss="alert">
              Send
            </button>
          </div>
        </form>
      </div>
    </div>

    <script>
      // Example starter JavaScript for disabling form submissions if there are invalid fields
      (function () {
        "use strict";
        window.addEventListener(
          "load",
          function () {
            // Fetch all the forms we want to apply custom Bootstrap validation styles to
            var forms = document.getElementsByClassName("needs-validation");
            // Loop over them and prevent submission
            var validation = Array.prototype.filter.call(
              forms,
              function (form) {
                form.addEventListener(
                  "submit",
                  function (event) {
                    if (form.checkValidity() === false) {
                      event.preventDefault();
                      event.stopPropagation();
                    }
                    form.classList.add("was-validated");
                  },
                  false
                );
              }
            );
          },
          false
        );
      })();
    </script>
  </body>
  <script
    src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
    integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
    crossorigin="anonymous"
  ></script>
  <script
    src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
    integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
    crossorigin="anonymous"
  ></script>
  <script
    src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
    integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
    crossorigin="anonymous"
  ></script>
</html>