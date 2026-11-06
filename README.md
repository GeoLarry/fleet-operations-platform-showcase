# Cartrace — screenshots

Cartrace is a fleet and vehicle-movement management app for car rental companies. Staff record vehicle pickups and deliveries with a full inspection: fuel and mileage, accessories, damages marked on a vehicle diagram, and the customer's signature. Each movement produces a PDF report in two languages.

The source code is private. This repository only holds screenshots of the running app. All data shown is fake, generated with Bogus.

## Tech stack

| Part | Technologies |
|---|---|
| Frontend | Angular 16 (NgModules, Angular Material), light and dark theme, Greek and English UI |
| Backend | .NET 10 Minimal API, clean architecture (Core / Infrastructure / API), JWT, permission-based RBAC |
| Reports | FastReport Open Source (PDF), SkiaSharp for the damage diagram |
| Demo data | Bogus |

## Movements

Movements list with search by license plate and date range. The actions on each row depend on the movement's state: open movements can be edited or deleted, completed ones can only be viewed or printed.

![Movements list](screenshots/01-movements-list.png)

The inspection form: general information, damages, accessories, notes and the customer's signature.

![Movement inspection form](screenshots/02-movement-inspection-form.png)

Damages are marked on a diagram of the vehicle and listed with their type, severity and billing (chargeable or not).

![Damage diagram](screenshots/03-damage-diagram.png)

Choosing a vehicle zone and the exact area of a new damage.

![Damage zone picker](screenshots/04-damage-zone-picker.png)

A completed movement opens read-only. It keeps the damages that were active at that time, even if they were repaired later.

![Completed movement preview](screenshots/05-completed-movement-preview.png)

Starting a new movement from a license plate (check-in or check-out), and finding a vehicle to manage its damages.

![New movement dialog](screenshots/06-new-movement-dialog.png)
![Damage management search](screenshots/07-damage-management-search.png)

## Fleet

![Fleet list](screenshots/08-fleet-list.png)

Vehicle details, editing and adding a new vehicle.

![Vehicle details](screenshots/09-vehicle-details.png)
![Vehicle edit](screenshots/10-vehicle-edit.png)
![New vehicle](screenshots/11-vehicle-new.png)

Damages belong to the vehicle. They can be recorded and marked as repaired from the fleet view as well, not only through a movement.

![Vehicle damages](screenshots/12-vehicle-damages.png)

## Users and roles

![Users](screenshots/13-users.png)
![User edit](screenshots/14-user-edit.png)

Custom roles grant permissions per module and action.

![Roles](screenshots/15-roles.png)
![Role permissions](screenshots/16-role-permissions.png)

## Dark theme

![Movements list, dark theme](screenshots/17-movements-list-dark.png)
![Movement inspection form, dark theme](screenshots/18-movement-inspection-form-dark.png)
![Fleet list, dark theme](screenshots/19-fleet-list-dark.png)
