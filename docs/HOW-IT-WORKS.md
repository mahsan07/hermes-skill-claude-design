# How Claude Design Works

Design one-off HTML artifacts such as landing pages, decks, and prototypes.

![Detailed systems blueprint for Claude Design](../assets/system-blueprint.png)

## Stages

### 1. Translate intent into visual hierarchy

**Primary surface:** `Design brief`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.
### 2. Choose typography color and spacing

**Primary surface:** `Content hierarchy`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.
### 3. Build the semantic HTML structure

**Primary surface:** `HTML and CSS composition`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.
### 4. Add responsive layout and interaction

**Primary surface:** `Responsive preview`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.
### 5. Render desktop and mobile previews

**Primary surface:** `One-off artifact`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.
### 6. Deliver the self-contained artifact

**Primary surface:** `One-off artifact`

Record the input, operation, observable output, and any decision that changes scope. Stop here if the output is missing, contradictory, or insufficient for the next stage.

## Failure handling

- **Authorization failure:** do not probe credentials or broaden access; report the missing authority.
- **Target ambiguity:** stop before mutation and request the minimum identifying information.
- **Tool or service failure:** retain error evidence, retry only safe transient failures, and cap retries.
- **Verification failure:** classify the run as incomplete even when the preceding operation returned success.

## Completion evidence

The handoff should contain the original request, inspection state, preview or plan, exact execution result, direct verification, and a final receipt naming limitations and withheld actions.
