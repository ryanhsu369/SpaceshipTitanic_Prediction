## Dataset Description

In this competition, your task is to predict whether a passenger was transported to an alternate dimension during the **Spaceship Titanic's** collision with a spacetime anomaly.

To help you make these predictions, you are given a set of personal records recovered from the ship's damaged computer system.

---

## File and Data Field Descriptions

### 📁 `train.csv`

Personal records for about two-thirds (~8,700) of the passengers, used as **training data**.

| Column Name | Description |
|------------|------------|
| PassengerId | A unique ID for each passenger. Format: `gggg_pp`, where `gggg` indicates the travel group and `pp` is the passenger number within the group. |
| HomePlanet | The planet the passenger departed from (usually their permanent residence). |
| CryoSleep | Whether the passenger was put into suspended animation during the voyage. |
| Cabin | Cabin number in the format `deck/num/side`, where side is `P` (Port) or `S` (Starboard). |
| Destination | The planet the passenger is traveling to. |
| Age | Age of the passenger. |
| VIP | Whether the passenger paid for special VIP service. |
| RoomService | Amount billed for room service. |
| FoodCourt | Amount billed at the food court. |
| ShoppingMall | Amount billed at the shopping mall. |
| Spa | Amount billed at the spa. |
| VRDeck | Amount billed at the VR deck. |
| Name | First and last name of the passenger. |
| Transported | **Target variable** — whether the passenger was transported to another dimension. |

---

### 📁 `test.csv`

Personal records for the remaining one-third (~4,300) of the passengers, used as **test data**.

- Contains the same columns as `train.csv`
- **Does not include** the `Transported` column
- Your task is to predict `Transported` for these passengers

---

### 📁 `sample_submission.csv`

Example submission file in the correct format.

| Column Name | Description |
|------------|------------|
| PassengerId | Passenger ID from the test set |
| Transported | Predicted value (`True` or `False`) |

## Sample Records

| PassengerId | Transported |
|------------|-------------|
| 0013_01 | False |
| 0018_01 | False |
| 0019_01 | False |
| 0021_01 | False |
| 0023_01 | False |
| 0027_01 | False |

